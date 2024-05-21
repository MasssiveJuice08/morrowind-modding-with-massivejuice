---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore-manual-entry/2024-03/abbreviations-web-accessibility-guidance-project-nz-government/","title":"Abbreviations — Web Accessibility Guidance project — NZ Government\n","metatags":{"description":"Make abbreviations accessible by providing or linking to the expanded form the first time it’s used on the page.","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["MMW-Dev/Workflow","MMW-Dev/CSS","MMW-Dev/Accessibility","omnivore-bug"]}
---


## Abbreviations — Web Accessibility Guidance project — NZ Government
#Omnivore

[Read on Omnivore](https://omnivore.app/me/abbreviations-web-accessibility-guidance-project-nz-government-18e750dd719)
[Read Original](https://govtnz.github.io/web-a11y-guidance/wct/abbreviations/)

### Highlights

> If an abbreviation has not become part of the language, provide one of the following in text right before or after the abbreviation’s first instance on the page:
> its expanded form
> an explanation of what the abbreviation means.
> Alternatively, link at least the first instance of the abbreviation to its expanded form or explanation elsewhere on the same or another page. [⤴️](https://omnivore.app/me/abbreviations-web-accessibility-guidance-project-nz-government-18e750dd719#13ee1944-974e-41df-939d-013d62e99e20) 
{ #13ee1944}


> some browsers display an `<abbr>` element that has a title attribute with a dotted underline, but this style can be changed by the page author.
> When an `<abbr>` element is hovered over with a mouse, the expanded form in the title attribute will display as a tooltip.
> If the abbreviation’s first instance on the page is accompanied by its expanded form, then all other instances of the abbreviation can be marked up using the `<abbr>` element without a title attribute. [⤴️](https://omnivore.app/me/abbreviations-web-accessibility-guidance-project-nz-government-18e750dd719#1a58ba0d-54b2-416f-baec-f6913ab5c5fb) 
{ #1a58ba0d}


> Why `<abbr>` is unreliable
> Unfortunately, the tooltip that’s provided to sighted mouse users when they hover over an `<abbr>` element with a title attribute is not provided to sighted keyboard or touch users. Also, screen reader support for `<abbr>` with title is inconsistent.
> As such, this approach cannot be relied on for exposing the expanded version of abbreviations to screen reader users. Instead, try to make sure that the first instance of the abbreviation on the page is accompanied by its fully expanded form or an explanation in text. [⤴️](https://omnivore.app/me/abbreviations-web-accessibility-guidance-project-nz-government-18e750dd719#39bf3f4a-9bce-4ed4-b730-0fdd0e3392b0) 
{ #39bf3f4a}


For abbreviations, the `<abbr>` element is useful but has limitations. First instances of abbreviations on a page should be supported by explanations in the text and/or by links to the full definition.

