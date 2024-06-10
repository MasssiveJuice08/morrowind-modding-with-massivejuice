---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore/2024-04/obsidian-grid-callouts-joschua-io/","title":"Obsidian Grid Callouts - joschua.io\n","metatags":{"description":"How to arrange content in Obsidian in columns without any plugins.","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["MMW-Dev/CSS","Obsidian/CSS"]}
---


## Obsidian Grid Callouts - joschua.io
#Omnivore

[Read on Omnivore](https://omnivore.app/me/obsidian-grid-callouts-joschua-io-18e9c3f29f0)
[Read Original](https://joschua.io/posts/2022/12/04/obsidian-grid-callouts/)

### Highlights

> ## Implementation
> 
> The two callouts that are displayed side by side are actually encapsulated by another callout. This callout arranges all its content in columns.
> 
> ![Obsidian note showing one larger callout containing two smaller ones within.](https://proxy-prod.omnivore-image-cache.app/1544x710,suVKYk4-4F3nlaaiyzMmiJOz6TYCfjhlxEemdsEzVfmo/https://joschua.io/_astro/5-even-columns.b06c2b03_Z1rHdJF.webp) [⤴️](https://omnivore.app/me/obsidian-grid-callouts-joschua-io-18e9c3f29f0#5ec2da49-9c5d-47f5-a9bf-1de87c206d57) 
{ #5ec2da49}


Article contains CSS snippets for grid callouts

> A [CSS snippet](https://help.obsidian.md/How+to/Add+custom+styles#Use+Themes+and+or+CSS+snippets) in Obsidian applies the styling.
> 
> `.obsidian/snippets/callouts.css`:
> 
> ```css
> /* Even columns */
> .callout[data-callout="even-columns"] {
>   /* Removes padding and background colour from the container */
>   padding: 0;
>   background-color: transparent;
> }
> .callout[data-callout="even-columns"] > .callout-content {
>   /* Arranges the content in columns */
>   display: grid;
>   /* minmax sets the minimum width of a column. Make the columns 'skinnier' by setting 15rem to a smaller number */
>   grid-template-columns: repeat(auto-fit, minmax(15rem, 1fr));
>   gap: 12px;
> }
> .callout[data-callout="even-columns"] > .callout-title {
>   /* Hides the callout title */
>   display: none;
> }
> ``` [⤴️](https://omnivore.app/me/obsidian-grid-callouts-joschua-io-18e9c3f29f0#bb441ba0-0bed-488a-86d0-cc488fa4e9b6) 
{ #bb441ba0}


Note that `grid-template-columns:` uses the ['repeat()' function](https://developer.mozilla.org/en-US/docs/Web/CSS/repeat), which "represents a repeated fragment of the track list, allowing a large number of columns that exhibit a recurring pattern to be written in a more compact form.

> The great thing about `grid` is that it is really flexible. Each new line in our callout automatically moves into a new column.
> 
> ```shell
> > [!even-columns]
> > left
> >
> > center
> >
> > right
> ```
> 
> ![Three columns in an Obsidian note.](https://proxy-prod.omnivore-image-cache.app/2400x1642,sf0oXcmLqPpqtbpqJpho5Z1MTKGNd82L_S2yOUPq5uQY/https://joschua.io/_astro/6-three.9861c745_ZVkmth.webp)
> 
> On a smaller display size, for example on mobile, the columns stack responsively depending on how much space is available. [⤴️](https://omnivore.app/me/obsidian-grid-callouts-joschua-io-18e9c3f29f0#1cc85032-564f-427e-bee3-fd0c7e6ba46a) 
{ #1cc85032}


This callout actually creates columns by default in the parent container call

