% Descriptive statistics
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

Description
-----------

This template will return descriptive statistics of a numerical
variable.

*age* ("Age")
-------------

The dataset has *709* observations with *677* valid values (missing:
*32*) in *age* ("Age"), which seems to be a quantitative variable.

### Base statistics

  **value**   **mean(age)**   **sd(age)**   **var(age)**
  ----------- --------------- ------------- --------------
  (all)       24.5731         6.8491        46.9107

### Histogram

![image](ac5d789145bdef09b10219ef16429f53.png)

It seems that the highest value is *58* which is exactly 3.625 times
higher than the smallest value (*16*).

The standard deviation is *6.8491* (variance: *46.9107*). The expected
value is around *24.5731*, somewhere between *24.0572* and *25.0891*
with the standard error of *0.2632*.

If we suppose that *Age* is not near to a normal distribution (test: see
below, skewness: *1.9296*, kurtosis: *7.4851*), checking the median
(*23*) might be a better option instead of the mean. The interquartile
range (*6*) measures the statistics dispersion of the variable (similar
to standard deviation) based on median.

### Normality tests

#### Introduction

In statistics, *normality* refers to an assumption that the distribution
of a random variable follows *normal* (*Gaussian*) distribution. Because
of its bell-like shape, it's also known as the *"bell curve"*. The
formula for *normal distribution* is:

$$f(x) = \frac{1}{\sqrt{2\pi{}\sigma{}^2}} e^{-\frac{(x-\mu{})^2}{2\sigma{}^2}}$$

*Normal distribution* belongs to a *location-scale family* of
distributions, as it's defined two parameters:

-   *μ* - *mean* or *expectation* (location parameter)
-   *σ^2^* - *variance* (scale parameter)

![image](2f8c434e103f36ec70966b372838d448.png)

#### Normality Tests

##### Overview

Various hypothesis tests can be applied in order to test if the
distribution of given random variable violates normality assumption.
These procedures test the H~0~ that provided variable's distribution is
*normal*. At this point only few such tests will be covered: the ones
that are available in `stats` package (which comes bundled with default
R installation) and `nortest` package that is
[available](http://cran.r-project.org/web/packages/nortest/index.html)
on CRAN.

-   **Shapiro-Wilk test** is a powerful normality test appropriate for
    small samples. In R, it's implemented in `shapiro.test` function
    available in `stats` package.
-   **Lilliefors test** is a modification of *Kolmogorov-Smirnov test*
    appropriate for testing normality when parameters or normal
    distribution (*μ*, *σ^2^*) are not known. `lillie.test` function is
    located in `nortest` package.
-   **Anderson-Darling test** is one of the most powerful normality
    tests as it will detect the most of departures from normality. You
    can find `ad.test` function in `nortest` package.
-   **Pearson Χ^2^ test** is another normality test which takes more
    "traditional" approach in normality testing. `pearson.test` is
    located in `nortest` package.

##### Results

Here you can see the results of applied normality tests (*p-values* less
than 0.05 indicate significant discrepancies):

*0.05*

So, let's draw some conclusions based on applied normality test:

-   according to *Shapiro-Wilk test*, the distribution of *Age* is not
    normal.
-   based on *Lilliefors test*, distribution of *Age* is not normal
-   *Anderson-Darling test* confirms violation of normality assumption
-   *Pearson's Χ^2^ test* classifies the underlying distribution as
    non-normal

#### Diagnostic Plots

There are various plots that can help you decide about the normality of
the distribution. Only a few most commonly used plots will be shown:
*histogram*, *Q-Q plot* and *kernel density plot*.

##### Histogram

*Histogram* was first introduced by *Karl Pearson* and it's probably the
most popular plot for depicting the probability distribution of a random
variable. However, the decision depends on number of bins, so it can
sometimes be misleading. If the variable distribution is normal, bins
should resemble the "bell-like" shape.

![image](ac5d789145bdef09b10219ef16429f53.png)

##### Q-Q Plot

"Q" in *Q-Q plot* stands for *quantile*, as this plot compares empirical
and theoretical distribution (in this case, *normal* distribution) by
plotting their quantiles against each other. For normal distribution,
plotted dots should approximate a "straight", `x = y` line.

![image](cbbba756d844aa053998959b73b9feff.png)

##### Kernel Density Plot

*Kernel density plot* is a plot of smoothed *empirical distribution
function*. As such, it provides good insight about the shape of the
distribution. For normal distributions, it should resemble the well
known "bell shape".

![image](168d92f4cf90d2c563e5a0166a64150c.png)

* * * * *

This report was generated in [R](http://www.r-project.org/) with
[Rapport](http://al3xa.github.com/rapport/) in 0.625 sec. Feel free to
create [your own reporting
templates](http://al3xa.github.com/rapport/#custom)!

![image](images/rapport.png)