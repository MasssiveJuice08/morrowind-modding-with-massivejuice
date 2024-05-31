---
{"dg-publish":true,"permalink":"/01-fleeting-notes/hamburger-menu-for-quartz/","metatags":{"description":"Notes on the potential implementation of a mobile hamburger menu for the Morrowind Modding Wiki","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["MMW-Dev/CSS","Quartz/CSS"]}
---

## About

As of writing (2024-05-31) the current version of [Quartz](https://github.com/jackyzha0/quartz) lacks a mobile hamburger menu. This makes navigation on mobile reliant on the (admittedly good) search function and the sensible placement of links by the creator of a given Quartz website. It's not ideal.

Some Quartz users have implemented a hamburger menu on their own website, such as [Owlly Lab](https://www.mara-li.fr/) by Mara-Li ([Github Repo](https://github.com/Mara-Li/owlly-lab)). Mara-Li added a [pull request to merge the burger menu](https://github.com/jackyzha0/quartz/pull/754) into Quartz, but it has issues that require resolving first before it can be merged:
- The burgerMenu layout requires a specific layout structure in a docstring in the layout.ts file in order to work.
- The code requires cleaning as it has a lot of duplicate code.

These issues don't prevent us from implementing it ourselves in the [[00 Projects/Morrowind Modding Wiki/Morrowind Modding Wiki - Home\|Morrowind Modding Wiki]], but it may be wise to instead wait for the official version to be merged.

As an alternative (or addition) to improve navigation on mobile, we could [[01 Fleeting Notes/Implementing a Horizontal Nav-Bar in Quartz\|implement a horizontal nav-bar]] that is pinned to the top of the page, with links to main sections of the wiki.