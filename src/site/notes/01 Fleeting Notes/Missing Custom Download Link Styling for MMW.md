---
{"dg-publish":true,"permalink":"/01-fleeting-notes/missing-custom-download-link-styling-for-mmw/","tags":["MMW-Style","MMW-Dev/CSS","Quartz/CSS"]}
---

## Issue

The [[00 Projects/Morrowind Modding Wiki/Morrowind Modding Wiki - Home\|Morrowind Modding Wiki]] uses `![[embedded files]]` to add download links inside articles. For example, the wiki article ['Tutorial - Create and ESP Replacer Patch'](https://morrowind-modding.github.io/Guides/Patches/Tutorial---Create-an-ESP-Replacer-Patch) includes a download link to a zip file containing the ESP files to be used alongside the tutorial. In Obsidian's default theme these are styled somewhat like a download link (though not _perfect_ - it uses a note 📄 symbol instead of a ⬇️ download symbol). However, Quartz styles these like a standard blockquote. This makes it difficult for readers to determine if this is a downloadable file or not, unless they click it.

### Default Quartz Styling for Transclusions

> [!caption|wmed right]
> 
> ![MMW_missing-custom-download-style.jpg|wm-sm right](/img/user/Assets/Fleeting/MMW_missing-custom-download-style.jpg)
> Quartz styles `![[embedded files]]` like blockquotes

[Quartz](https://quartz.jzhao.xyz/) handles the styling of embedded files (termed 'transclusions' by Quartz) in different ways depending on the file extension type. This is handled by the [ObsidianFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/ObsidianFlavoredMarkdown) Quartz plugin (`quartz/plugins/transformers/ofm.ts`). Some examples include:
- Images (e.g., `.png`) are embedded in the web page
- Audio (e.g., `mp3`) and video (e.g., `.wav`) files are placed in a controllable media player
- PDFs get embedded as an HML `<iframe>`

However, all other embedded file extension types are styled as a blockquotes, including zip files. A download link is inserted with the `<data-url>` HTML tag.

---

> [!caption|wfull]
> 
> ![Quartz_styling_embedded_zip-file_download_as_blockquote.png](/img/user/Assets/Fleeting/Quartz_styling_embedded_zip-file_download_as_blockquote.png)
> Zip files within blockquotes in Quartz are downloadable via the `<data-url>` HTML tag.

## Solution

Using CSS, we should be able to add custom styling to embedded downloadable files.