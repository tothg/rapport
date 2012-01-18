% t-test Template
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

## Description

A t-test report with table of descriptives, diagnostic tests and t-test
specific statistics.

# Introduction

In a nutshell, *t-test* is a statistical test that assesses hypothesis
of equality of two means. But in theory, any hypothesis test that yields
statistic which follows
[*t-distribution*](https://en.wikipedia.org/wiki/Student's_t-distribution)
can be considered a *t-test*. The most common usage of *t-test* is to:

-   compare the mean of a variable with given test mean value -
    **one-sample *t-test***
-   compare means of two variables from independent samples -
    **independent samples *t-test***
-   compare means of two variables from dependent samples -
    **paired-samples *t-test***

# Overview

Independent samples *t-test* is carried out with *Internet usage in
leisure time (hours per day)* as dependent variable, and *Gender* as
independent variable. Confidence interval is set to 95%. Equality of
variances wasn't assumed.

# Descriptives

In order to get more insight on the underlying data, a table of basic
descriptive statistics is displayed below.

  **y**    **min(x)**   **max(x)**   **mean(x)**   **sd(x)**   **var(x)**   **median(x)**   **IQR(x)**   **skewness(x)**   **kurtosis(x)**
  -------- ------------ ------------ ------------- ----------- ------------ --------------- ------------ ----------------- -----------------
  male     0            12           3.2699        1.9535      3.8161       3               3            0.9479            4.0064
  female   0            12           3.0643        2.3546      5.5442       2               3            1.4064            4.9089
           0            10           3.3824        2.5822      6.6676       3               2            1.2197            3.8058

# Diagnostics

Since *t-test* is a parametric technique, it sets some basic assumptions
on distribution shape: it has to be *normal* (or appoximately normal). A
few normality test are to be applied, in order to screen possible
departures from normality.

## Normality Tests

We will use *Shapiro-Wilk*, *Lilliefors* and *Anderson-Darling* tests to
screen departures from normality in the response variable (*Internet
usage in leisure time (hours per day)*).

<!-- endlist -->

                 **W**    **p**
  -------------- -------- -------
  shapiro.test   0.9001   0
  lillie.test    0.168    0
  ad.test        18.753   0

As you can see, applied tests confirm departures from normality.

# Results

Welch Two Sample t-test was applied, and significant differences were
found.

<!-- endlist -->

      **statistic**   **df**     **p**    **CI(lower)**   **CI(upper)**
  --- --------------- ---------- -------- --------------- ---------------
  t   1.1483          457.8625   0.2514   -0.1463         0.5576

## Description

A t-test report with table of descriptives, diagnostic tests and t-test
specific statistics.

# Introduction

In a nutshell, *t-test* is a statistical test that assesses hypothesis
of equality of two means. But in theory, any hypothesis test that yields
statistic which follows
[*t-distribution*](https://en.wikipedia.org/wiki/Student's_t-distribution)
can be considered a *t-test*. The most common usage of *t-test* is to:

-   compare the mean of a variable with given test mean value -
    **one-sample *t-test***
-   compare means of two variables from independent samples -
    **independent samples *t-test***
-   compare means of two variables from dependent samples -
    **paired-samples *t-test***

# Overview

One-sample *t-test* is carried out with *Internet usage in leisure time
(hours per day)* as dependent variable. Confidence interval is set to
95%. Equality of variances wasn't assumed.

# Descriptives

In order to get more insight on the underlying data, a table of basic
descriptive statistics is displayed below.

# Diagnostics

Since *t-test* is a parametric technique, it sets some basic assumptions
on distribution shape: it has to be *normal* (or appoximately normal). A
few normality test are to be applied, in order to screen possible
departures from normality.

## Normality Tests

We will use *Shapiro-Wilk*, *Lilliefors* and *Anderson-Darling* tests to
screen departures from normality in the response variable (*Internet
usage in leisure time (hours per day)*).

<!-- endlist -->

                 **W**    **p**
  -------------- -------- -------
  shapiro.test   0.9001   0
  lillie.test    0.168    0
  ad.test        18.753   0

As you can see, applied tests confirm departures from normality.

# Results

One Sample t-test was applied, and significant differences were found.

<!-- endlist -->

      **statistic**   **df**   **p**    **CI(lower)**   **CI(upper)**
  --- --------------- -------- -------- --------------- ---------------
  t   -0.0072         671      0.9943   3.037           3.3618

* * * * *

This report was generated with [rapport](http://rapport-package.info/).

![image](images/rapport.png)