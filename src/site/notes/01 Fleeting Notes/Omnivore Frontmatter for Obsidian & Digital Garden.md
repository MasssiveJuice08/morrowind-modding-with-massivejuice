---
{"dg-publish":true,"permalink":"/01-fleeting-notes/omnivore-frontmatter-for-obsidian-and-digital-garden/","tags":["My-Website"]}
---

## Publishing Omnivore notes from Obsidian to Digital Garden



### About

I use [Omnivore](https://omnivore.app/) to save articles and documents while researching a topic. It allows me to tag ('label') them, highlight passages and add notes to my highlights. I'm a pretty forgetful person and with ADHD my brain is working like, what, 512mb of RAM anyway? Citing my sources 

The challenge I have encountered with publishing my  notes is that if a note gets resynced, it overrides the frontmatter. Digital Garden 

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