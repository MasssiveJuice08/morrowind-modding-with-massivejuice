---
{"dg-publish":true,"permalink":"/01-fleeting-notes/omnivore-frontmatter-for-obsidian-and-digital-garden/","metatags":{"description":"How I publish Onnivore article highlights from Obsidian to my Digital Garden","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["My-Website"]}
---

## Publishing Omnivore notes from Obsidian to Digital Garden

[![Omnivore.app Logo|right wsmall](https://i.imgur.com/0YszZiM.png)](https://omnivore.app/)

The challenge I have encountered with publishing my notes synced from Omnivore is that if a note gets resynced, it overrides the frontmatter. Digital Garden relies on adding the frontmatter `dg-publish: true` to notes in order to publish them, and this gets removed during the resync. Thankfully there's a workaround – Omnivore's Obsidian plugin allows you to customise the frontmatter template for synced articles using the [Mustache](https://mustache.github.io/mustache.5.html) language, so I added the following lines to the template:

```
dg-publish: true
dg-metatags:
 description: "{{{description}}}"
 "og:image": "https://i.imgur.com/LmCg5HX.png"
```

As well as `dg-publish`, I also added `dg-metatags` which help with SEO and populate links to the relevant page with a short description. In this case, the `{{{description}}}` Mustache tag tells Obsidian to use the description of the synced article from Omnivore.

My full frontmatter template is below:

```
id: {{{id}}}
title: >
  {{{title}}}
{{#author}}
author: >
  {{{author}}}
{{/author}}
{{#labels.length}}
tags:
{{#labels}} - {{{name}}}
{{/labels}}
{{/labels.length}}
date_saved: {{{dateSaved}}}
{{#datePublished}}
date_published: {{{datePublished}}}
{{/datePublished}}
site_name: {{siteName}}
original_url: {{{omnivoreUrl}}}
dg-publish: true
dg-metatags:
 description: "{{{description}}}"
 "og:image": "https://i.imgur.com/LmCg5HX.png"
```