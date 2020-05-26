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
Recently SCB, the Swedish bureau of statistics releasaed all-cause mortality for March and most of April. It's hard to estimate just how deadly COVID-19 is, to ascertain what epidemiologists call Infection-fatality Rate, one needs the true number of deaths, and the true number of cases. This is hard. Another way is to to look at Mortality rate, and compare it to previous years. This has several strengths. First of all, it will capture second-order effects. As hospitals are increasingly strained by the large number of cases, other medical procedures will be delayed. People might be afraid to go to the hospital the check out that chest pain. By looking at daily deaths, these effects will be reflected in the data.



We start by by taking a look on number of daily deaths for the years 2015-2020.
For 2020, the data for all of april has not been released yet. Furthermore, it takes a couple of weeks for the numbers to be correct for any particular date. This can be seen in the graph as the line trending downwards and the end of April. SCB released the latest daily death statistics the 27th of April, but in the following graphs the data will only be visualized up until the 15th of April.




<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-2-1.png" width="672" />

We can see a sharp uptick in April of 2020. Lets compare just this period to 2018 and 2019. The graphs show data until the 16th of April, where the number of deaths per day is growing much smaller due to the lag effect.

<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-3-1.png" width="672" />



The data shows that all-cause mortality for all of Sweden starts to rise in the end of March. But how many more people have actually died? Below is the number of deaths between the 1th of January and April 20th.


```
## # A tibble: 6 x 2
##    year `sum(Deaths)`
##   <dbl>         <dbl>
## 1  2015         30282
## 2  2016         28747
## 3  2017         29771
## 4  2018         30967
## 5  2019         27592
## 6  2020         30261
```

Up until the 20th of April, more people actually had died in 2018 or 2015 than in 2020.
March the 11th was date of the first person to die of COVID-19. Lets restrict the range to start at that period.



```
## # A tibble: 6 x 2
##    year `sum(Deaths)`
##   <dbl>         <dbl>
## 1  2015         10125
## 2  2016          9586
## 3  2017          9529
## 4  2018         10469
## 5  2019          9163
## 6  2020         11970
```

In this timeperiod, the total number of deaths is higher for 2020. Compared to 2015 and 2018, who likely had more severe flu epidemics, 2020 has ~1300 more deaths than 2018, and ~1600 more deaths than 2015.


However, viruses like COVID - 19 grow in clusters, and some areas will be much farther along in the epidemic than others.

Let's break down the analysis by County. First, let us take a look at Stockholm, the worst hit county in Sweden.



```
## Warning: Removed 1 row(s) containing missing values (geom_path).
```

<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-7-1.png" width="672" />

The impact on excess deaths are pretty obvious in  s Stockholm. How about the other countys?
<img src="/post/2020-05-26-excess-deaths-in-sweden_files/figure-html/unnamed-chunk-8-1.png" width="672" />

This is interesting! The only county with a clear elevated daily death statistic is Stockholm.
The pandemic doesnt seem to have a very large impact on number of deaths outside of Stockholm.

