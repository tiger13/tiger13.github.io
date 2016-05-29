---
title       : Probability from the Logistic Function
subtitle    : 
author      : tiger13
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax, quiz, bootstrap]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## The Logistic Function

The logistic function is given by this equation

$$P = \frac{1}{1 + e^{-(a + b x)}}$$

where $a$ and $b$ are constants.

--- .class #id 

## Class Probabilities 

This equation can be used to model the probability of belonging to one of two classes. For a given value of $x$, the probability of belonging to the first class is $P$, and the probability of belonging to the second class is $1 - P$.

---

## Example

If $a = 1$, $b = 0.5$, and $x = 0.25$, the probability of belonging  to the first class can be calculated as follows:

```r
a <- 1
b <- 0.5
x <- 0.25
P <- 1/(1 + exp(-a - b * x))
```
And the probability is 0.754915.

--- &radio

## Question 1

What is the probability for $a = 1$, $b = 0.5$, and $x = 0.5$?

1. 0.75

2. _0.78_

3. 0.25

4. 1.0

*** .hint

The probability should be close, but not equal, to the value calculated in the example.

*** .explanation

0.78

--- 
