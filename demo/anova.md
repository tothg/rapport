% ANOVA Template
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

Description
-----------

An ANOVA report with table of descriptives, diagnostic tests and
ANOVA-specific statistics.

Introduction
------------

**Analysis of Variance** or **ANOVA** is a statistical procedure that
tests equality of means for several samples. It was first introduced in
1921. by famous English statistician Sir Ronald Aylmer Fisher.

Model Overview
--------------

One-Way ANOVA was carried out, with *Gender* as independent variable,
and *Internet usage in leisure time (hours per day)* as a response
variable. Factor interaction was taken into account.

Descriptives
------------

In order to get more insight on the model data, a table of frequencies
for ANOVA factors is displayed, as well as a table of descriptives.

### Frequency Table

Below lies a frequency table for factors in ANOVA model. Note that the
missing values are removed from the summary.

  **gender**   **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------ ------- --------- -------------- --------------
  male         410     60.9212   410            60.9212
  female       263     39.0788   673            100
  Total        673     100       673            100

### Descriptive Statistics

The following table displays the descriptive statistics of ANOVA model.
Factor levels and/or their combinations lie on the left hand side, while
the corresponding statistics for response variable are given on the
right-hand side.

  **Gender**   **Min**   **Max**   **Mean**   **Std.Dev.**   **Median**   **IQR**   **Skewness**   **Kurtosis**
  ------------ --------- --------- ---------- -------------- ------------ --------- -------------- --------------
  male         0         12        3.2699     1.9535         3            3         0.9443         0.9858
  female       0         12        3.0643     2.3546         2            3         1.3979         1.8696

Diagnostics
-----------

Before we carry out ANOVA, we'd like to check some basic assumptions.
For those purposes, normality and homoscedascity tests are carried out
alongside several graphs that may help you with your decision on model's
main assumptions.

### Diagnostics

#### Univariate Normality

We will use *Shapiro-Wilk*, *Lilliefors* and *Anderson-Darling* tests to
screen departures from normality in the response variable (*Internet
usage in leisure time (hours per day)*).

<!-- endlist -->

                                                   **Statistic**   **p-value**
  ------------------------------------------------ --------------- -------------
  Shapiro-Wilk normality test                      0.9001          0
  Lilliefors (Kolmogorov-Smirnov) normality test   0.168           0
  Anderson-Darling normality test                  18.753          0

As you can see, applied tests confirm departures from normality.

#### Homoscedascity

In order to test homoscedascity, *Bartlett* and *Fligner-Kileen* tests
are applied.

<!-- endlist -->

                                                     **Statistic**   **p-value**
  -------------------------------------------------- --------------- -------------
  Fligner-Killeen test of homogeneity of variances   0.4629          0.4963
  Bartlett test of homogeneity of variances          10.7698         0.001

When it comes to equality of variances, applied tests yield inconsistent
results. While *Fligner-Kileen test* confirmed the hypotheses of
homoscedascity, *Bartlett's test* rejected it.

### Diagnostic Plots

Here you can see several diagnostic plots for ANOVA model:

-   residuals against fitted values
-   scale-location plot of square root of residuals against fitted
    values
-   normal Q-Q plot
-   residuals against leverages

[![image](dd5cdfe79c3741b4373910424cb2824c.png)](dd5cdfe79c3741b4373910424cb2824c-hires.png)

ANOVA Summary
-------------

### ANOVA Table

<!-- endlist -->

              **Df**   **Sum.Sq**   **Mean.Sq**   **F.value**   **Pr..F.**
  ----------- -------- ------------ ------------- ------------- ------------
  gender      1        6.4217       6.4217        1.4302        0.2322
  Residuals   636      2855.63      4.49                        

*F-test* for *Gender* is not statistically significant, which implies
that there is no Gender effect on response variable.

Description
-----------

An ANOVA report with table of descriptives, diagnostic tests and
ANOVA-specific statistics.

Introduction
------------

**Analysis of Variance** or **ANOVA** is a statistical procedure that
tests equality of means for several samples. It was first introduced in
1921. by famous English statistician Sir Ronald Aylmer Fisher.

Model Overview
--------------

Two-Way ANOVA was carried out, with *Gender* and *Relationship status*
as independent variables, and *Internet usage in leisure time (hours per
day)* as a response variable. Factor interaction was taken into account.

Descriptives
------------

In order to get more insight on the model data, a table of frequencies
for ANOVA factors is displayed, as well as a table of descriptives.

### Frequency Table

Below lies a frequency table for factors in ANOVA model. Note that the
missing values are removed from the summary.

  **gender**   **partner**         **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------ ------------------- ------- --------- -------------- --------------
  male         in a relationship   150     23.6967   150            23.6967
  female       in a relationship   120     18.9573   270            42.654
  male         married             33      5.2133    303            47.8673
  female       married             29      4.5814    332            52.4487
  male         single              204     32.2275   536            84.6761
  female       single              97      15.3239   633            100
  Total        Total               633     100       633            100

### Descriptive Statistics

The following table displays the descriptive statistics of ANOVA model.
Factor levels and/or their combinations lie on the left hand side, while
the corresponding statistics for response variable are given on the
right-hand side.

  **Gender**   **Relationship status**   **Min**   **Max**   **Mean**   **Std.Dev.**   **Median**   **IQR**   **Skewness**   **Kurtosis**
  ------------ ------------------------- --------- --------- ---------- -------------- ------------ --------- -------------- --------------
  male         in a relationship         0.5       12        3.0582     1.9692         2.5          2         1.3239         2.6488
  male         married                   0         8         2.9848     2.029          3            2         0.862          0.1509
  male         single                    0         10        3.5027     1.9361         3            3         0.7574         0.0875
  female       in a relationship         0.5       10        3.0439     2.2158         3            3         1.3833         1.8306
  female       married                   0         10        2.4808     1.9671         2            1.75      2.0626         5.5858
  female       single                    0         12        3.3226     2.6791         3            3.5       1.1851         0.9281

Diagnostics
-----------

Before we carry out ANOVA, we'd like to check some basic assumptions.
For those purposes, normality and homoscedascity tests are carried out
alongside several graphs that may help you with your decision on model's
main assumptions.

### Diagnostics

#### Univariate Normality

We will use *Shapiro-Wilk*, *Lilliefors* and *Anderson-Darling* tests to
screen departures from normality in the response variable (*Internet
usage in leisure time (hours per day)*).

<!-- endlist -->

                                                   **Statistic**   **p-value**
  ------------------------------------------------ --------------- -------------
  Shapiro-Wilk normality test                      0.9001          0
  Lilliefors (Kolmogorov-Smirnov) normality test   0.168           0
  Anderson-Darling normality test                  18.753          0

As you can see, applied tests confirm departures from normality.

#### Homoscedascity

In order to test homoscedascity, *Bartlett* and *Fligner-Kileen* tests
are applied.

<!-- endlist -->

                                                     **Statistic**   **p-value**
  -------------------------------------------------- --------------- -------------
  Fligner-Killeen test of homogeneity of variances   1.1234          0.2892
  Bartlett test of homogeneity of variances          11.1267         0.0009

When it comes to equality of variances, applied tests yield inconsistent
results. While *Fligner-Kileen test* confirmed the hypotheses of
homoscedascity, *Bartlett's test* rejected it.

### Diagnostic Plots

Here you can see several diagnostic plots for ANOVA model:

-   residuals against fitted values
-   scale-location plot of square root of residuals against fitted
    values
-   normal Q-Q plot
-   residuals against leverages

[![image](3e897b547f80202649804e256107f6e0.png)](3e897b547f80202649804e256107f6e0-hires.png)

ANOVA Summary
-------------

### ANOVA Table

<!-- endlist -->

                   **Df**   **Sum.Sq**   **Mean.Sq**   **F.value**   **Pr..F.**
  ---------------- -------- ------------ ------------- ------------- ------------
  gender           1        4.9473       4.9473        1.0853        0.2979
  partner          2        31.2124      15.6062       3.4237        0.0332
  gender:partner   2        3.0375       1.5188        0.3332        0.7168
  Residuals        593      2703.0899    4.5583                      

*F-test* for *Gender* is not statistically significant, which implies
that there is no Gender effect on response variable. Effect of
*Relationship status* on response variable is significant. Interaction
between levels of *Gender* and *Relationship status* wasn't found
significant (p = 0.717).

* * * * *

This report was generated with [R](http://www.r-project.org/) (2.14.0)
and [rapport](http://al3xa.github.com/rapport/) (0.2) in 1.82 sec on
x86\_64-unknown-linux-gnu platform.

![image](images/logo.png)