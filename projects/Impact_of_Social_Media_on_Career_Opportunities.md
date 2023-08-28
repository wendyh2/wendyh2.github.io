---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Impact of **Social Media** on Career Opportunities"
date: 2022-10-30
published: true
labels:
  - Social Media
  - Career
summary: "I created a website discussing the positive and negative impacts of social media on one's future job endeavors."
---

The website explores how social media, particularly in the business and marketing realm, can both positively and negatively impact career opportunities. It highlights platforms like LinkedIn, Indeed, Glassdoor, and Instagram as tools for self-marketing in job searches. LinkedIn is lauded for its networking potential, enabling users to build portfolios, connect with peers, access job insights, and communicate with recruiters. Instagram's significance for small businesses is underscored, exemplified by nail shops using the platform for customer engagement. While technology presents avenues for professional growth, the site also highlights the need for responsible online behavior to avoid detriments to job prospects. Ultimately, social media is portrayed as a valuable tool, contingent on ethical and strategic usage, for enhancing career possibilities in the discussed field.

Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
