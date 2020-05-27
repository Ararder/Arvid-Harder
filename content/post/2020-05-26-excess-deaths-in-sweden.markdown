---
title: Excess deaths in Sweden
author: ''
date: '2020-05-26'
slug: excess-deaths-in-sweden
categories: []
tags: []
subtitle: ''
summary: ''
authors: []
lastmod: '2020-05-26T22:07:37+02:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---





As of writing this, [Folkhälsomyndigheten](https://experience.arcgis.com/experience/09f821667ce64bf7be6f9f87457ed9aa) (FHM), the swedish institution for public health has reported 4125 deaths due to COVID-19. However, we know that the number of deaths due to COVID-19 is higher. Some people are bound to die before getting tested, and will not be counted in official statistics. And there is bound to be second-order effects. If you are 55 and feel a sharp pain in the left side of your chest, maybe you think twice about going to the hopsital. 


To get around this, another way of measuring death statistics is by looking at excess mortality. This compares the number of deaths this year, compared to other years. If we assume that the main difference between 2020 and other years is the COVID-19 pandemic, we can attribute the difference to corona! It is of course not possible to say that 2019 and 2020 is perfectly alike except in the case of a global pandemic. But estimating deaths this way is a better estimate than using official statistics. To get a feeling for how the mortality rate differs by year, let's start by looking at the number of daily deaths in Sweden, for the period 2015 - 2020. The data used in this analysis is provided by SCB. Since the start of the pandemic, it's been clear that these deaths sometimes take a while to be reported. Therefore, i show data up until May 8th, using the data published by SCB on May 22th. The two week delay should make the numbers shown robust to large reporting lags.
<p>&nbsp;</p>  


<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-2-1.png" width="672" />

The impact of COVID-19 is clear. Before March, 2020 is on track to have the lowest level of daily deaths in the period 2015-2020. The year that most closely follows the trajectory of 2020 is 2019. Somewhere around the 10th of March, the number of daily deaths sharply increases and peaks at April 15th with 397 deaths (Note that the graph shows a rolling 7-day average). The number of daily deaths then goes down following the peak, and seems to be on a steady decrease.


How the pandemic spreads differ a lot by city and country.
For example, New York has 29451 deaths according to [worldometer](https://www.worldometers.info/coronavirus/country/us/), which is a third of the entire US deathtoll. Regional mortality data is only publicaly available for 2018, 2019 and 2020. Therefore, let's take look at how these three years compare to each other in daily mortality.
<p>&nbsp;</p>  


<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-3-1.png" width="672" />

The main take-away from this graph is that 2018 is a relative outlier compared to 2020 and 2019. Up until middle of March, 2020 closely tracks the trajectory of 2019. When estimating excess deaths, i will give numbers with both 2018 and 2019 as comparisons, but i consider 2019 a better comparison to 2020 than 2018. While graphs are good to understand the trend, what does the numbers say?



| Year| Deaths|
|----:|------:|
| 2018|  35656|
| 2019|  32344|
| 2020|  36644|

2020 has about a thousand more deaths compared to 2018, and about 4000 thousand more deaths than 2019. However, the first reported death due to COVID-19 was on March 11th. Since we are interested in estimating excess deaths due to the pandemic, we can restrict the range where we count daily deaths. For this table, the range is between March 11th and May 8th. 


| Year| Deaths|
|----:|------:|
| 2018|  15476|
| 2019|  14181|
| 2020|  18580|

By restricting the range, the difference between 2018 and 2019 is no longer as large. The difference in deaths between 2019 and 2020 is also largely the same, indicating that most of the difference is from differences in mortality after March 11th. For 2018, the difference compared to 2020 is now much larger. This makes sense, as the impact of the flu epidemic of 2018 started fall of beginning in mid March if one looks at the previous graph.


Compared to confirmed deaths, the number of excess deaths are larger. According to Folkhälsomyndigheten, the number of confirmed deaths by May 8th was 3462. Using 2019 as a control group, the number of excess deaths are 4399, and if we use 2018 as comparison, the number of excess deaths are 3104. This is another point in favour of not using 2018 as a comparison. The number of excess deaths are lower than confirmed cases! This is not what we would expect given that 2018 and 2020 mainly differ in that 2020 has a global pandemic. 


Using the 2019 as comparison, Sweden had 4399 excess deaths. That's actually not to bad, compared to the numbers coming of out some other [countries](https://www.ft.com/content/4a91a414-4937-4c54-aa78-6d231f4a4e43). This would indicate that Sweden is pretty good at correctly labeling COVID-19 deaths.














Lets switch gears and look at these number, but on the level of the 21 Swedish counties. As we saw earlier, there is a huge variation between cities in the same country.


<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-10-1.png" width="672" />

 Only Stockholm has an obvious increase in mortality!

<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-11-1.png" width="672" />

| Year| Deaths|
|----:|------:|
| 2018|   2653|
| 2019|   2427|
| 2020|   4507|


The difference in total deaths for the time period March 11th - May 8th, is about 2000, for both 2018 and 2019 as comparisons! The flu pandemic of 2018 seems to have had less an impact in Stockholm. For this timeperiod the total number of deaths increased by 86% compared to 2019, and Stockholm stood for about half the excess mortality in Sweden, with only 1/5 the population!

We can calculate the same percetange for all the other counties. How much is the total number of deaths elevated in this time period?



|County         | % increase in deaths|
|:--------------|--------------------:|
|Stockholm      |                   86|
|Gotland        |                   61|
|Södermanland   |                   53|
|Dalarna        |                   46|
|Västmanland    |                   38|
|Östergötland   |                   37|
|Uppsala        |                   35|
|Jönköping      |                   28|
|VästraGötaland |                   26|
|Norrbotten     |                   22|
|Örebro         |                   19|
|Kalmar         |                   18|
|Halland        |                   15|
|VästerNorrland |                   14|
|Gävleborg      |                   13|
|Jämtland       |                   12|
|Kronoberg      |                   12|
|Skåne          |                    9|
|Blekinge       |                    7|
|Värmland       |                    1|
|Västerbotten   |                   -3|

We can take a closer look on the four counties with the highest percentage of increased number of deaths.

<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-13-1.png" width="672" />

Zooming, we can see that excess mortality starts to rise in the end of March. The numbers for Gotland is hard to visualize, as the county is so small that on most days nobody has died.

However, the population is Sweden is concetrated in its five largest counties, with the five largest counties accounting for 60% of the population. Zooming in, we could see that excess mortality is definitely up for several counties. How about the largest ones?

 
<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-14-1.png" width="672" />





# Conclusions

The excess mortality for Stockholm is quite large. Between the time period March 11th to May 8th, approximately 2100 more people died compared to the same time period in 2019. This corresponds to an increase of 86%. However, there is good news as the excess mortality seems to have peaked in the middle of April and has been on a steady trajectory downwards since then.

Other counties also show evidence of excess mortality, with Sörmland at an increase of 51% percent, and Dalarna at 46%. This highlights how affected Stockholm has been compared to other counties. For the four largest counties outside of Stockholm, the excess mortality is not at all as large as the other counties discussed. This is both good and bad news, depending on what strategy Sweden takes going forward. These results would indicate that some regions have not been hit hard at all, opening up the possibility of completely suppresing COVID-19. However, if Sweden decides to pursue a herd-immunity strategy for the whole country, some counties have the brunt of the epidemic in front of them.
 
