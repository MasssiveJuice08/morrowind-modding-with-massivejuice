---
{"dg-publish":true,"permalink":"/01-fleeting-notes/report-a-problem-button-for-mmw/","tags":["MMW-Dev/Workflow","Quartz/UI"]}
---

[Modding-OpenMW](https://modding-openmw.com/) uses a 'Report a Problem' button on content pages, which links directly to the Gitlab repository's Issues page.

<iframe src="https://modding-openmw.com/cfg-generator/" title="Modding OpenMW CFG Generator" width=100% height=500 style="border: 2px solid;"></iframe>

MMW could incorporate the same feature, directing users to the Github repository's Issues page. However, considering that [Giscus](https://github.com/giscus/giscus) comments have already been integrated, this could be 'double handling'. Giscus may also be better suited, as comments on a page open a Github Discussion focused specifically on the topic of that page.