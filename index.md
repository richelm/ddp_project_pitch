---
title       : Exploring Linear Models with MTCARS Dataset
subtitle    : 
author      : Shawn Rich
job         : Data Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---


## Motivation

Understanding linear models can be difficult. This shiny application is designed to help students learning linear models. Through the application interface, students interactively explore building and analyzing a linear model using the mtcars dataset. 

Key features of the application:

1. Variable transmission (am) is inlcuded in all models.
1. Checkbox inputs allow students to select additional variables from the dataset for their models.
1. Model summary and plots are generate for student review.
1. Help tab provides additional application information and explanation of mtcars dataset.


--- .class #id 

## Why Include Transmission Type in All Models?

Is there a difference in mean mpg for automatic and manual transmissions? A t-test shows that a null hypothesis of means being equal should be rejected.



```
## 
## 	Welch Two Sample t-test
## 
## data:  mpg.auto and mpg.manual
## t = -3.7671, df = 18.332, p-value = 0.001374
## alternative hypothesis: true difference in means is not equal to 0
## 95 percent confidence interval:
##  -11.280194  -3.209684
## sample estimates:
## mean of x mean of y 
##  17.14737  24.39231
```

We include *am* variable in all models and let the user of the application explore the other variables to determine which also predict miles per gallon.


--- .class #id 

## Intended Use

This application is designed to supplement an introductory course in regression models. It is assumed the course would cover the following topics:

* t Confidence intervals
* Hypothesis testing
* Ordinary least squares
* Regression to the mean
* Statistical linear regression models
* Residuals
* Plots of linear models


--- .class #id 

## Going Further

The application is is licensed under the terms of the MIT license. Expand the features for the mtcars dataset or add additional datasets for your students. Fork or clone from the following github repo:

[https://github.com/richelm/ddp](https://github.com/richelm/ddp)



