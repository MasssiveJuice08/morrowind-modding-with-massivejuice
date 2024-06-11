---
{"dg-publish":true,"permalink":"/01-fleeting-notes/kbd-html-element-in-markdown/","tags":["MMW-Dev/Accessibility","MMW-Dev/CSS","MMW-Style"]}
---

## About

the `<kbd> </kbd>` HTML element is used to denote keyboard input (such as "ctrl + alt + del"). Markdown uses backticks to define \`code\`, which in practice is a catch-all for `<kbd>`, `<samp>` (sample computer code output), and `code` HTML elements. By default, the aforementioned HTML elements are styled the same by default, but can be made to be rendered differently. Github renders `<kbd>` elements differently from \`code\`, but Obsidian does not do so by default.

> See this stackoverflow answer: [What are the differences between kbd, samp and code in HTML](https://stackoverflow.com/a/32284528) 

> [!Note] Consider adding custom CSS for \<kbd\> in MMW
> 
> This would improve readability, as currently there is no distinction between code and keyboard input.
> 
> ---
> 
> **Update: 2024-05-29:** `kbd` styling added to Morrowind Modding Wiki by commit [97e55f8](https://github.com/morrowind-modding/morrowind-modding.github.io/commit/97e55f8065ded2f699dbc0110995ce49630b7b55)

> [!tip]
> 
> HTML is a bitch to type out -- [\<kbd\> Generator \</kbd\>](https://kbd.hsuan.xyz/) is a useful tool to easily format and style \<kbd\> though it is Mac-focused and has limited input options (only key-press input is allowed)
> 
> [Github Source Code](https://github.com/hsuanxyz/kbd-generator)

