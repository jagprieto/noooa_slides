---
title       : Visualization of USA NOAA Storm Database
subtitle    : Population health and economics damages of USA NOAA Storm Database from 1993 to 2011
author      : José Antonio González Prieto
job         : Developing data products (Coursera 2014)
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## USA NOAA Storm Database

1.- USA NOAA Storm database tracks characteristics of major storms and weather events in the United States, including when and where they occur, as well as estimates of any fatalities, injuries, and property damage.

2.- A complete report with the exploratory data analysis and the getting and cleaning data process is available at [report link](http://rpubs.com/jagprieto/23612).


3.- Final report containts 14 event types created at the exploratory data analysis.

4. Work created for the Peer Assessment 2 at the Reproducible Research course in Coursera (Jul 2014).

--- .class #id 


## Injuries and fatalities summary

1. The TORNADO event type is the principal cause of injuries and fatalities. 
2. Event types WIND and STORM causes no large peaks, so it accumulates data with less variation that the other event types.
3. Event types HEAT and FLOOD ocasionally appears and causes a considerable increment in the number of injuries and fatalities but very concentrated in time.
4.  Event types AVALANCHE and SURF has a superior ratio of fatalities versus injuries, which implies that this kind of events are qualitive (not quantitative) more dangerous.
5.  Event type HURRICANE causes less injuries/fatalitites than expected if we think about the nature of the event, but we must also consider the possibility of prediction of this kind of events which help us to save lives.
6.  The difficult to predict AVALANCHE and SURF could also be a good clue to understand why this kind of events have the highest dangerous ratios.

--- .class #id 

## Damages summary

1. The STORM event type is the principal cause of damages, altough it was not one of the principal causes in population health.
2. The HURRICANE, TORNADO AND FLOOD event types causes almost the total of the non STORM damages.
3. We can observe that the most dangerous events: AVALANCHE and SURF have a low impact in the economics results.

The mean as standard deviation of damages in million dollars by state are:  Mean = 4553.45,  Standard deviation = 9308.21 .

--- .class #id 


## USA geographic summary
1. States TX, LA, OK, AR, MO, IA, MN, WI, IL, TN, AL, GA, MI, KY, OH, FL, PA and NC concentrates the mayor impact events with respect to population health. 
2. The mean as standard deviation of injuries are: Mean = 2332.10 and  Standard deviation = 3109.75. 
3. The mean as standard deviation of fatalities are: Mean = 41.97 and  Standard deviation = 303.66 . 
4. The south east region (LA, TX, AL, MS, FL) have the larger impact in ecomonomics because of climatic events.
5. The mean as standard deviation of damages in million dollars by state are: Mean  = 4553.45, Standard deviation = 9308.21 .


--- .class #id 
 
 
## USA NOAA Storm visualizer
Shiny application that includes the possibility to filter information based on:

1. Population health and economics damages : fatalities, injuries, and damages.
2. Year range from 1993 to 2011 (where the information is more reliable.
3. Accumulative (from 1993) or independent year data visualization.
4. Bar plot with event type distribution or USA map distribution.
5. General statistics (median, variance, max and min values).

Available at : [NOAA visualizer](https://jagprieto.shinyapps.io/NOOA_VISUALIZER/)
