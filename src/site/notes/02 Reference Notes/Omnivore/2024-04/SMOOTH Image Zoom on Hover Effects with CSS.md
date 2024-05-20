---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore/2024-04/smooth-image-zoom-on-hover-effects-with-css/","title":"SMOOTH Image Zoom on Hover Effects with CSS\n","metatags":{"description":"A bunch of instant CSS recipes to achieve slick image hover zoom effects coupled with some rotation, scaling, blurring, and more.","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["CSS","MMW-Style"]}
---


## SMOOTH Image Zoom on Hover Effects with CSS
#Omnivore

[Read on Omnivore](https://omnivore.app/me/https-w-3-bits-com-css-image-hover-zoom-18f1a310388)
[Read Original](https://w3bits.com/css-image-hover-zoom/)

### Highlights

> We need a container element which will be hovered and then the image inside it should animate accordingly, i.e. zoom-in or zoom-out as per the need.
> 
> Note that the image should zoom on hover inside the container element and do not come or flow outside of it when it gets zoomed.
> 
> So, the basic idea is to limit the container element with the CSS **overflow** property.
> 
> The zooming and animation parts will be handled with the CSS3 **transform** and **transition** properties respectively. [⤴️](https://omnivore.app/me/https-w-3-bits-com-css-image-hover-zoom-18f1a310388#a153adb4-d0dc-4350-8b02-08bff4dd091c) 
{ #a153adb4}


How to create on-hover image zoom container

> ### The CSS
> 
> Observe the below CSS.
> 
> ```css
> /* [1] The container */
> .img-hover-zoom {
>   height: 300px; /* [1.1] Set it as per your need */
>   overflow: hidden; /* [1.2] Hide the overflowing of child elements */
> }
> 
> /* [2] Transition property for smooth transformation of images */
> .img-hover-zoom img {
>   transition: transform .5s ease;
> }
> 
> /* [3] Finally, transforming the image when container gets hovered */
> .img-hover-zoom:hover img {
>   transform: scale(1.5);
> }
> ```
> 
> ####  [⤴️](https://omnivore.app/me/https-w-3-bits-com-css-image-hover-zoom-18f1a310388#d6b6103b-04dc-43fd-8504-0790ea08a3fb) 
{ #d6b6103b}


#CSS

