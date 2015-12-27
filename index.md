---
title       : Intro to MPG Prediction
subtitle    : A shiny application
author      : smilelee725   
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Goal
MPG prediction application is to predict the MPG based on the user's car configuration.



--- .class #id 

## Approach
* Application built in Shiny.
* Use mtcars dataset.
* Use linear regression model to make prediction.  
  + A prediction function is built internally

```r
predict_mpg<-function(i_cyl = 6,i_hp = 110,i_wt = 3.0,i_am = 1)
```



--- .class #id

## Example

We have a dataset

```r
v<-data.frame(cyl = 6,hp = 150, wt = 2.7, am = 1)
```
Type the above dataset into the corresponding fields in application and click *Go MPG!*  
We get 20.93 MPG as prediction on the right side.  

Note that horsepower and weight have range of acceptable values.  
* horsepower between 50 and 400.
* weight between 1 and 10.

--- .class #id

## Conclusion
MPG prediction is an easy to use application to help predict MPG for your car.  

