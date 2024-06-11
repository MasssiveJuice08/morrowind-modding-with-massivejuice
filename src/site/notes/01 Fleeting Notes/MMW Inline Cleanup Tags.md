---
{"dg-publish":true,"permalink":"/01-fleeting-notes/mmw-inline-cleanup-tags/","metatags":{"description":"","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["MMW-Policy"]}
---


## About

Wikipedia uses what it calls ['inline-cleanup tags'](https://en.wikipedia.org/wiki/Template:Inline_cleanup_tags) to mark sections of text which require revision.

In appearance, these are similar to footnotes – a piece of superscript surrounded by square brackets.[^1] Where they differ is that they are names, contain a hyperlink to the definition of the cleanup tag in question, and words within the square brackets are italicised.

Some common examples include:

- <sup>\[_[according to whom?](https://en.m.wikipedia.org/wiki/Wikipedia:Manual_of_Style/Words_to_watch#Unsupported_attributions)_\]</sup>
- <sup>\[_[original research?](https://en.m.wikipedia.org/wiki/Wikipedia:No_original_research)_\]</sup>
- <sup>\[_[citation needed](https://en.m.wikipedia.org/wiki/Wikipedia:Citation_needed)_\]</sup>

For the [[00 Projects/Morrowind Modding Wiki/Morrowind Modding Wiki - Home\|Morrowind Modding Wiki]], these would help to identify specific sections requiring attention. 

Implementing them is thankfully possible by mixing a little be of HTML with Markdown:

### HTML Superscript Tags

Obsidian-Flavored Markdown accepts the superscript HTML tag ('`<sup> </sup>`').

In practice, superscript reduces the font size, raises the line height and (optionally) changes the font of a string of text. Wikilinks and external links can be rendered inside the tags, and the text can also be styled with standard Markdown.<sup>\[_[super important tag](https://youtu.be/dQw4w9WgXcQ?si=TrWb1BFdT2XsjvyG)_\]</sup>

The Markdown, for internal and external links respectively, is formatted like so:

```
<sup>\[_[[name of tag]]_\]</sup>

<sup>\[_[name of tag](url)_\]</sup>
```

The HTML method is functional, but tedious to format. this could be alleviated by creating templates for the tags, possibly even using [Templater](https://github.com/SilentVoid13/Templater) so that the tags can be inserted around a highlighted string of text.


[^1]: This is a footnote
