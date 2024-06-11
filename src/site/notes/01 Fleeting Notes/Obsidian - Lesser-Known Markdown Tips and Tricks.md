---
{"dg-publish":true,"permalink":"/01-fleeting-notes/obsidian-lesser-known-markdown-tips-and-tricks/","metatags":{"description":"Exploring the more obscure features of Obsidian Markdown formatting","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["Obsidian"]}
---

## About

Not all of Obsidian's capabilities are thoroughly documented in the [Obsidian Help Docs](https://help.obsidian.md/Home).

That's not to say that the docs are lacking – they are an excellent primer on using Obsidian. What is lacking is some of the more particular, obscure workarounds inherent to [Markdown](https://www.markdownguide.org/) and HTML content in Markdown. These are generally for very specific use-cases.

## Display a Link as an Image

> [!caption|wmed right]
> 
> [![An image as a clickable link|wm-m](https://i.imgur.com/bdAW9ne.png)](https://morrowind-modding-with-massivejuice.vercel.app/)
> 
> A link displayed as an image – clicking the link will take you to the homepage. 

Want to create a button or an image that links to a different note or an external web page?

We can do this by wrapping an embedded image inside the square brackets (`[ ]`) of a standard [Markdown link](https://www.markdownguide.org/basic-syntax/#links). Inside the square brackets we would insert the Markdown for either:

- an embedded [Internal Image](https://help.obsidian.md/Linking+notes+and+files/Embed+files#Embed+an+image+in+a+note), e.g:

```
![[Engelbart.jpg]]
```

- an [External Image](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#External+images), e.g:

```
![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

### External Link

Using an image to link to an external web page:

**Eternal image:**

```Markdown 
[![image alt text](url to image)](https://www.some-website.com)
```

**Internal image** embedded via `wikilink`:

```Markdown
[![[wikilink to image.png]]](https://www.some-website.com)
```

### Internal Link

Using an image to link to an internal page does not work using the standard `[[wikilink]]` syntax. 

Instead, it is formatted like a Markdown link, with the exception that instead of a URL in the `(brackets)`, you would put the page name surrounded by `< >`. So, `[[page title]]`  would instead be written as `(<page title>)`

Here is the full formatting:

**Eternal image:**

```Markdown 
[![image alt text](url to image)](<page name>)
```

**Internal image** embedded via `wikilink`:

```Markdown
[![[wikilink to image.png]]](<page name>)
```

---

## Wikipedia-Style 'Inline Cleanup Tags'

Using the HTML `<sup>` (superscript) tag, we can create a Wikipedia-style [Inline Cleanup Tag](https://en.wikipedia.org/wiki/Template:Inline_cleanup_tags).

You may have seen them before while trawling a wiki article – they look like this:

- Some consider the Tribunal to be false gods. <sup>\[_[according to whom?](https://en.m.wikipedia.org/wiki/Wikipedia:Manual_of_Style/Words_to_watch#Unsupported_attributions)_\]</sup>
- Wulfharth, along with Dagoth Ur, led the Nordic and Orc forces into Morrowind. <sup>\[_[original research?](https://en.m.wikipedia.org/wiki/Wikipedia:No_original_research)_\]</sup>
- Nerevar was betrayed and murdered by the Tribunal. <sup>\[_[citation needed](https://en.m.wikipedia.org/wiki/Wikipedia:Citation_needed)_\]</sup>

> [!note|clean embed no-t] 
> 
> 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/01-fleeting-notes/mmw-inline-cleanup-tags/#html-superscript-tags" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# clean

</div>


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


</div></div>

