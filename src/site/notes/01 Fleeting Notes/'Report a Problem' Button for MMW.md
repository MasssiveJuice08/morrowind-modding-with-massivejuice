---
{"dg-publish":true,"permalink":"/01-fleeting-notes/report-a-problem-button-for-mmw/","tags":["MMW-Dev/Workflow","Quartz/UI"]}
---

## Use-Case for a 'Report a Problem' Button for the Morrowind Modding Wiki:

[Modding-OpenMW](https://modding-openmw.com/) uses a 'Report a Problem' button on selected pages, such as the [CFG Generator](https://modding-openmw.com/cfg-generator/), which links directly to the Gitlab repository's Issues page.

> [!caption]
> 
> ![Report-a-problem-MOMW-button.jpg](/img/user/Assets/Fleeting/Report-a-problem-MOMW-button.jpg)
> 
> Selected pages on [MOMW](https://modding-openmw.com/) contain a 'Report a Problem' button.

MMW could incorporate the same feature, directing users to the Github repository's Issues page. However, considering that [Giscus](https://github.com/giscus/giscus) comments have already been integrated, this could be 'double handling'. Giscus may also be better suited, as comments on a page open a Github Discussion focused specifically on the topic of that page.

On the other hand, opening a new Github issue for each reported bug or typo relating to a single page might make for easier issue tracking than having everything contained within a single discussion thread. Furthermore, the Giscus Discussions won't only be used for bug tracking, so searching for reported problems may be more dofficult due to needing to scroll through a number of unrelated comments. A 'Report a Problem' button could be a valuable addition to supplement this.