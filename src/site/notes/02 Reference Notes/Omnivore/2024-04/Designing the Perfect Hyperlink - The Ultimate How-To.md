---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore/2024-04/designing-the-perfect-hyperlink-the-ultimate-how-to/","title":"Designing the Perfect Hyperlink - The Ultimate How-To\n","metatags":{"description":"The design of hyperlinks can affect the usability of your web pages and also the user experience. Here are some tips to improve hyperlink designs.","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["MMW-Dev/CSS","CSS/Hyperlinks","MMW-Dev/Accessibility"]}
---


## About

#Omnivore

[Read on Omnivore](https://omnivore.app/me/designing-the-perfect-hyperlink-the-ultimate-how-to-18e981945be)
[Read Original](https://www.webfx.com/blog/web-design/hyperlink-design/)

The design of hyperlinks can affect the usability of your web pages and also the user experience. Here are some tips to improve hyperlink designs.

_This page is powered by [Omnivore](https://omnivore.app) ‐ you can read more about how I use Omnivore here: [[02 Reference Notes/Omnivore/Omnivore - Saving Articles for Citations in Obsidian\|Omnivore - Saving Articles for Citations in Obsidian]]._

### Highlights

> Hyperlinks Need to Look Like Hyperlinks
>  All your hyperlinks need to stand out and clearly say to your readers, “Hey I’m a link. You can click on me.” Hyperlinks should appear interactable.
>  As web designers, we like to innovate and experiment with different navigation techniques, but sticking with certain design conventions is important. One of the things that need to remain conventional is our hyperlinks. According to a study in link readability, the regular Web user sees blue-and-underlined text as links.
>  Blue and underlined is a good standard to stick to, for no other reason than it’s what we Internet users have been acclimatized ourselves to. [⤴️](https://omnivore.app/me/designing-the-perfect-hyperlink-the-ultimate-how-to-18e981945be#4747fe6c-c23d-4ee6-bf98-aac072b31e09) 
{ #4747fe6c}


Hyperlinks should be underlined and blue because it is the standard convention.

> [There is a study](https://vsis-www.informatik.uni-hamburg.de/getDoc.php/publications/119/www2003.pdf) that shows that **readability decreases when we underline the text** in our hyperlinks. The study says that underlined links have “_seriously underestimated effects on the usability of Web pages._” The study reports that our current convention of underlining hyperlinks “_can significantly reduce the readability of the text._” [⤴️](https://omnivore.app/me/designing-the-perfect-hyperlink-the-ultimate-how-to-18e981945be#18f718e3-14f8-47b8-b2b4-15ef36f6c582) 
{ #18f718e3}


The standard convention is flawed - underlined text can reduce readability.

> #### What’s the Solution to This Readability Issue?
> 
>  We can fix this readability issue ourselves. We don’t have to wait for a change in the way web browsers render underlined text by default. How?
> 
>  We can use the CSS `border-bottom` property instead of the CSS `text-decoration` property to underline our hyperlink elements. Using the `border-bottom` property can place the underline a few pixels below the affected characters, making the hyperlink easier to read. ![0357 09 default hyperlink borderbottom](https://proxy-prod.omnivore-image-cache.app/549x279,sV3NOB6cVhc6nrCyEmDIzDuRk20RCB9kd3vwho7miGYE/https://www.webfx.com/wp-content/uploads/2021/10/0357-09_default_hyperlink_borderbottom.png) [⤴️](https://omnivore.app/me/designing-the-perfect-hyperlink-the-ultimate-how-to-18e981945be#8460fd60-26e0-4b50-b0a2-05b5806f4d5f) 
{ #8460fd60}


Add padding to make the underline sit further below the text so it doesn't cut through characters.

> Even more powerful than just fixing a readability issue, we can also control the underline’s style independently from the hyperlink text color, thereby decoupling these two components of a hyperlink.
> 
>  For example, we can reduce the hyperlink underline’s [distinctiveness](https://www.webfx.com/blog/web-design/the-art-of-distinction-in-web-design/) to make the text more legible, or we can make it more distinctive to make the entire hyperlink design really stand out. [⤴️](https://omnivore.app/me/designing-the-perfect-hyperlink-the-ultimate-how-to-18e981945be#0e67604d-48de-41a3-89fd-60cfd8575289) 
{ #0e67604d}


Make underline colour subtly different from hyperlink text to improve distinctiveness and readability. 

