---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore-manual-entry/2024-03/html-what-is-the-benefit-to-using-acronym-and-abbreviation-html-tags-stack-overflow/","title":"HTML - What is the benefit to using Acronym and Abbreviation HTML Tags - Stack Overflow","metatags":{"description":"A Stack Overflow discussion on the use of acronym and abbreviation HTML tags","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["Obsidian/CSS","MMW-Dev/SEO","omnivore-bug"]}
---


## html - What is the benefit to using <acronym> and <abbr>? - Stack Overflow
#Omnivore

[Read on Omnivore](https://omnivore.app/me/html-what-is-the-benefit-to-using-acronym-and-abbr-stack-overflo-18e74691668)
[Read Original](https://stackoverflow.com/questions/2196980/what-is-the-benefit-to-using-acronym-and-abbr)

### Highlights

> There is likely to be no or infinitesimally small SEO benefit from using these tags unless the abbreviation is not well known or something you made up or there is some ambiguity. For example, in an article about LILO the Linux Loader, you may want to specify `<acronymtitle="Linux Loader">LILO</acronym>` to avoid confusion with Last In, Last Out.
> Any accessibility benefit would exist only for those acronyms and abbreviations that are not well known by the target audience. For instance, it makes very little to no sense to have `<abbr lang="en"title="Mister">Mr.</abbr>` (WCAG checkpoint 4.2 disagrees with me on this. Note also that I did not provide an expansion of WCAG in my post).
> On the other hand, if you use are not using IMF to refer to the International Monetary Fund, it might make sense to use `<acronym lang="en"title="Impossible Mission Force">IMF</acronym>`.
> Now, what happens if you also want to use IMF to mean International Monetary Fund in the same document?
> The article The Accessibility Hat Trick: Getting Abbreviations Right might also be useful.
> Interesting nuggets:
> The assertion that abbr is structural is misguided, as the point of the tag is the content of its title attribute.
> ...
> In [XHTML] version 2, the acronym element has been deprecated, so we're now using the abbr element for all shortened forms. [⤴️](https://omnivore.app/me/html-what-is-the-benefit-to-using-acronym-and-abbr-stack-overflo-18e74691668#593b5ff9-e387-450b-a7fa-b34a33e9ca54) 
{ #593b5ff9}


