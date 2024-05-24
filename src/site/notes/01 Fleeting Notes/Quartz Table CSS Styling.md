---
{"dg-publish":true,"permalink":"/01-fleeting-notes/quartz-table-css-styling/","tags":["Quartz/CSS","MMW-Dev/CSS"]}
---

## About

Quartz by default uses a very clean styling for its tables, which includes not using vertical pipes between table columns. This looks slick, but may not increase readability,

I found someone else's Quartz table styling which includes a checker-styled pattern background, and rows get highlighted when `on-hover` (not pictured).

![Fancy_checker-styled_tables_for_Quartz.png|center](/img/user/Assets/Fleeting/Fancy_checker-styled_tables_for_Quartz.png)

### Source: 

https://discord.com/channels/927628110009098281/927628110009098284/1197643806883991632

> "For example for the table `tab.MCMC.a` for the `<table>...</table>` section, given I, was already working in `R`, and because I am Lazy I used `cat(knitr::kable(tab.MCMC.a, "html"), sep = "\n")`. then I i just appended some custom style if necessary in `<head><style>...</style></head>` otherwise I have styles set at `quartz/styles/custom.scss `"

```
/* Styles for Light Theme */
[saved-theme="light"] table {
  /* Light theme table styles */
  background-color: #ffffff; /* white background for light theme */
  color: #000000; /* black text for light theme */
  border-collapse: collapse;
  width: 90%;
  margin-left: auto; 
  margin-right: auto; 
  
  td {
    padding: 8px;
    text-align: left;
    border-bottom: 1px solid #CFE4FF;
  }
  
  tr:nth-child(even) td {
    background-color: #f9f9f9;
  }
  
  tr:hover td {
    background-color: #f1f1f1;
  }
  
  th {
    text-align: center; 
    padding: 8px; 
    font-size: 16.5px;
  }

  caption {
    padding: 8px;
    font-size: larger;
    caption-side: top;
  }
}



/* Styles for Dark Theme */
[saved-theme="dark"] {
  table {
    background-color: #36312A; /* dark gray background for dark theme */
    color: #ffffff; /* white text for dark theme */
    border-collapse: collapse;
    width: 90%;
    margin-left: auto;
    margin-right: auto;

    td {
      padding: 8px;
      text-align: center;
      border-bottom: 1px solid #A19084;
    }

    tr:nth-child(even) td {
      background-color: #2B2519;
    }

    th {
    text-align: center; 
    padding: 8px; 
    font-size: 16.5px;
  }

    tr:hover td {
      background-color: #4F483E;
    }

    caption {
      padding: 8px;
      font-size: larger;
      caption-side: top;
    }
  }
}
```