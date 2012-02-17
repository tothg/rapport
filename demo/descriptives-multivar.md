% Descriptive statistics
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

Description
-----------

This template will return descriptive statistics of numerical or
frequency tables of categorical variables.

*gender* ("Gender")
-------------------

The dataset has *709* observations with *673* valid values (missing:
*36*) in *gender* ("Gender"), which seems to be a qualitative variable.

### Base statistics

  **gender**   **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------ ------- --------- -------------- --------------
  male         410     60.9212   410            60.9212
  female       263     39.0788   673            100
  Total        673     100       673            100

### Barplot

[![image](3a46554ee29cd4dfe45dda5016464658.png)](3a46554ee29cd4dfe45dda5016464658-hires.png)

It seems that the highest value is *2* which is exactly 2 times higher
than the smallest value (*1*).

The most frequent value is *male*.

*age* ("Age")
-------------

The dataset has *709* observations with *677* valid values (missing:
*32*) in *age* ("Age"), which seems to be a quantitative variable.

### Base statistics

  **Variable**   **mean**   **sd**   **var**
  -------------- ---------- -------- ---------
  Age            24.5731    6.8491   46.9107

### Histogram

[![image](4f025d440bf35d40e21208e8b0c58b77.png)](4f025d440bf35d40e21208e8b0c58b77-hires.png)

It seems that the highest value is *58* which is exactly 3.625 times
higher than the smallest value (*16*).

The standard deviation is *6.8491* (variance: *46.9107*). The expected
value is around *24.5731*, somewhere between *24.0572* and *25.0891*
with the standard error of *0.2632*.

If we suppose that *Age* is not near to a normal distribution (test: see
below, skewness: *1.9254*, kurtosis: *4.463*), checking the median
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

[![image](806ea97c59e1a12d4acae4968957aaa9.png)](806ea97c59e1a12d4acae4968957aaa9-hires.png)

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

<!-- endlist -->

                                                   **Statistic**   **p-value**
  ------------------------------------------------ --------------- -------------
  Shapiro-Wilk normality test                      0.8216          0
  Lilliefors (Kolmogorov-Smirnov) normality test   0.17            0
  Anderson-Darling normality test                  32.1645         0
  Pearson chi-square normality test                625.8479        0

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

[![image](4f025d440bf35d40e21208e8b0c58b77.png)](4f025d440bf35d40e21208e8b0c58b77-hires.png)

##### Q-Q Plot

"Q" in *Q-Q plot* stands for *quantile*, as this plot compares empirical
and theoretical distribution (in this case, *normal* distribution) by
plotting their quantiles against each other. For normal distribution,
plotted dots should approximate a "straight", `x = y` line.

[![image](131f20f388f78bd4863828d9fed8c35c.png)](131f20f388f78bd4863828d9fed8c35c-hires.png)

##### Kernel Density Plot

*Kernel density plot* is a plot of smoothed *empirical distribution
function*. As such, it provides good insight about the shape of the
distribution. For normal distributions, it should resemble the well
known "bell shape".

[![image](b721e8de05c207e4bb17bbf28c7edda8.png)](b721e8de05c207e4bb17bbf28c7edda8-hires.png)

Description
-----------

This template will return descriptive statistics of numerical or
frequency tables of categorical variables.

*chatim* ("Chat & IM usage")
----------------------------

The dataset has *709* observations with *669* valid values (missing:
*40*) in *chatim* ("Chat & IM usage"), which seems to be a qualitative
variable.

### Base statistics

  **chatim**    **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         60      8.9686    60             8.9686
  very rarely   73      10.9118   133            19.8804
  rarely        58      8.6697    191            28.5501
  sometimes     113     16.8909   304            45.441
  often         136     20.3288   440            65.7698
  very often    88      13.154    528            78.9238
  always        141     21.0762   669            100
  Total         669     100       669            100

### Barplot

[![image](a3a825d8535e7c9b8a9d23cc8c1293b1.png)](a3a825d8535e7c9b8a9d23cc8c1293b1-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *always*.

*game* ("On-line games usage")
------------------------------

The dataset has *709* observations with *677* valid values (missing:
*32*) in *game* ("On-line games usage"), which seems to be a qualitative
variable.

### Base statistics

  **game**      **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         352     51.9941   352            51.9941
  very rarely   128     18.9069   480            70.901
  rarely        32      4.7267    512            75.6278
  sometimes     60      8.8626    572            84.4904
  often         37      5.4653    609            89.9557
  very often    35      5.1699    644            95.1256
  always        33      4.8744    677            100
  Total         677     100       677            100

### Barplot

[![image](601bf73b7f424e34c795446ca73a1bac.png)](601bf73b7f424e34c795446ca73a1bac-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *never*.

*surf* ("Web surfing usage")
----------------------------

The dataset has *709* observations with *678* valid values (missing:
*31*) in *surf* ("Web surfing usage"), which seems to be a qualitative
variable.

### Base statistics

  **surf**      **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         17      2.5074    17             2.5074
  very rarely   26      3.8348    43             6.3422
  rarely        33      4.8673    76             11.2094
  sometimes     107     15.7817   183            26.9912
  often         158     23.3038   341            50.295
  very often    142     20.944    483            71.2389
  always        195     28.7611   678            100
  Total         678     100       678            100

### Barplot

[![image](8b8013a5d21daf05463bf12edc7d6bfa.png)](8b8013a5d21daf05463bf12edc7d6bfa-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *always*.

*email* ("Email usage")
-----------------------

The dataset has *709* observations with *672* valid values (missing:
*37*) in *email* ("Email usage"), which seems to be a qualitative
variable.

### Base statistics

  **email**     **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         13      1.9345    13             1.9345
  very rarely   36      5.3571    49             7.2917
  rarely        46      6.8452    95             14.1369
  sometimes     87      12.9464   182            27.0833
  often         123     18.3036   305            45.3869
  very often    108     16.0714   413            61.4583
  always        259     38.5417   672            100
  Total         672     100       672            100

### Barplot

[![image](7d530054059115b70f8098f2e3ff6c81.png)](7d530054059115b70f8098f2e3ff6c81-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *always*.

*download* ("Download usage")
-----------------------------

The dataset has *709* observations with *677* valid values (missing:
*32*) in *download* ("Download usage"), which seems to be a qualitative
variable.

### Base statistics

  **download**   **N**   **%**     **Cumul. N**   **Cumul. %**
  -------------- ------- --------- -------------- --------------
  never          11      1.6248    11             1.6248
  very rarely    28      4.1359    39             5.7607
  rarely         29      4.2836    68             10.0443
  sometimes      80      11.8168   148            21.8612
  often          124     18.3161   272            40.1773
  very often     160     23.6337   432            63.8109
  always         245     36.1891   677            100
  Total          677     100       677            100

### Barplot

[![image](c5c68401731dd8623c3bac532d4f93b1.png)](c5c68401731dd8623c3bac532d4f93b1-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *always*.

*forum* ("Web forums usage")
----------------------------

The dataset has *709* observations with *673* valid values (missing:
*36*) in *forum* ("Web forums usage"), which seems to be a qualitative
variable.

### Base statistics

  **forum**     **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         76      11.2927   76             11.2927
  very rarely   80      11.8871   156            23.1798
  rarely        72      10.6984   228            33.8782
  sometimes     111     16.4933   339            50.3715
  often         109     16.1961   448            66.5676
  very often    119     17.682    567            84.2496
  always        106     15.7504   673            100
  Total         673     100       673            100

### Barplot

[![image](e866a67bba62e7f5cbe93b184599019f.png)](e866a67bba62e7f5cbe93b184599019f-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *very often*.

*socnet* ("Social networks usage")
----------------------------------

The dataset has *709* observations with *678* valid values (missing:
*31*) in *socnet* ("Social networks usage"), which seems to be a
qualitative variable.

### Base statistics

  **socnet**    **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         208     30.6785   208            30.6785
  very rarely   102     15.0442   310            45.7227
  rarely        57      8.4071    367            54.1298
  sometimes     87      12.8319   454            66.9617
  often         79      11.6519   533            78.6136
  very often    80      11.7994   613            90.413
  always        65      9.587     678            100
  Total         678     100       678            100

### Barplot

[![image](6619f2daf580503ce53708176cb0d83b.png)](6619f2daf580503ce53708176cb0d83b-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *never*.

*xxx* ("Adult sites usage")
---------------------------

The dataset has *709* observations with *674* valid values (missing:
*35*) in *xxx* ("Adult sites usage"), which seems to be a qualitative
variable.

### Base statistics

  **xxx**       **N**   **%**     **Cumul. N**   **Cumul. %**
  ------------- ------- --------- -------------- --------------
  never         274     40.6528   274            40.6528
  very rarely   124     18.3976   398            59.0504
  rarely        52      7.7151    450            66.7656
  sometimes     131     19.4362   581            86.2018
  often         46      6.8249    627            93.0267
  very often    28      4.1543    655            97.181
  always        19      2.819     674            100
  Total         674     100       674            100

### Barplot

[![image](cbda2b116fe3f7095f2997068f945424.png)](cbda2b116fe3f7095f2997068f945424-hires.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *never*.

Description
-----------

This template will return descriptive statistics of numerical or
frequency tables of categorical variables.

*hp*
----

The dataset has *32* observations with *32* valid values (missing: *0*)
in *hp*, which seems to be a quantitative variable.

### Base statistics

  **Variable**   **mean**   **sd**    **var**
  -------------- ---------- --------- -----------
  hp             146.6875   68.5629   4700.8669

### Histogram

[![image](78517cde85fc1ba06a3513dd17e567da.png)](78517cde85fc1ba06a3513dd17e567da-hires.png)

It seems that the highest value is *335* which is exactly 6.4423 times
higher than the smallest value (*52*).

The standard deviation is *68.5629* (variance: *4700.8669*). The
expected value is around *146.6875*, somewhere between *122.9317* and
*170.4433* with the standard error of *12.1203*.

If we suppose that *hp* is not near to a normal distribution (test: see
below, skewness: *0.726*, kurtosis: *-0.1356*), checking the median
(*123*) might be a better option instead of the mean. The interquartile
range (*83.5*) measures the statistics dispersion of the variable
(similar to standard deviation) based on median.

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

[![image](806ea97c59e1a12d4acae4968957aaa9.png)](806ea97c59e1a12d4acae4968957aaa9-hires.png)

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

<!-- endlist -->

                                                   **Statistic**   **p-value**
  ------------------------------------------------ --------------- -------------
  Shapiro-Wilk normality test                      0.9334          0.0488
  Lilliefors (Kolmogorov-Smirnov) normality test   0.1664          0.0245
  Anderson-Darling normality test                  0.7077          0.0584
  Pearson chi-square normality test                11.5            0.0423

So, let's draw some conclusions based on applied normality test:

-   according to *Shapiro-Wilk test*, the distribution of *hp* is not
    normal.
-   based on *Lilliefors test*, distribution of *hp* is not normal
-   *Anderson-Darling test* confirms normality assumption
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

[![image](78517cde85fc1ba06a3513dd17e567da.png)](78517cde85fc1ba06a3513dd17e567da-hires.png)

##### Q-Q Plot

"Q" in *Q-Q plot* stands for *quantile*, as this plot compares empirical
and theoretical distribution (in this case, *normal* distribution) by
plotting their quantiles against each other. For normal distribution,
plotted dots should approximate a "straight", `x = y` line.

[![image](1cefec04e4451a937a5c6aa4dfdcb352.png)](1cefec04e4451a937a5c6aa4dfdcb352-hires.png)

##### Kernel Density Plot

*Kernel density plot* is a plot of smoothed *empirical distribution
function*. As such, it provides good insight about the shape of the
distribution. For normal distributions, it should resemble the well
known "bell shape".

[![image](edfab5d9e83f64514100b0acc016dbea.png)](edfab5d9e83f64514100b0acc016dbea-hires.png)

*wt*
----

The dataset has *32* observations with *32* valid values (missing: *0*)
in *wt*, which seems to be a quantitative variable.

### Base statistics

  **Variable**   **mean**   **sd**   **var**
  -------------- ---------- -------- ---------
  wt             3.2172     0.9785   0.9574

### Histogram

[![image](bf47295875cfa6d1667455a7d2721b19.png)](bf47295875cfa6d1667455a7d2721b19-hires.png)

It seems that the highest value is *5.424* which is exactly 3.5849 times
higher than the smallest value (*1.513*).

The standard deviation is *0.9785* (variance: *0.9574*). The expected
value is around *3.2172*, somewhere between *2.8782* and *3.5563* with
the standard error of *0.173*.

If we suppose that *wt* is not near to a normal distribution (test: see
below, skewness: *0.4231*, kurtosis: *-0.0227*), checking the median
(*3.325*) might be a better option instead of the mean. The
interquartile range (*1.0288*) measures the statistics dispersion of the
variable (similar to standard deviation) based on median.

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

[![image](806ea97c59e1a12d4acae4968957aaa9.png)](806ea97c59e1a12d4acae4968957aaa9-hires.png)

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

<!-- endlist -->

                                                   **Statistic**   **p-value**
  ------------------------------------------------ --------------- -------------
  Shapiro-Wilk normality test                      0.9433          0.0927
  Lilliefors (Kolmogorov-Smirnov) normality test   0.1356          0.1412
  Anderson-Darling normality test                  0.6091          0.1038
  Pearson chi-square normality test                4.5             0.4799

So, let's draw some conclusions based on applied normality test:

-   according to *Shapiro-Wilk test*, the distribution of *wt* is
    normal.
-   based on *Lilliefors test*, distribution of *wt* is not normal
-   *Anderson-Darling test* confirms normality assumption
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

[![image](bf47295875cfa6d1667455a7d2721b19.png)](bf47295875cfa6d1667455a7d2721b19-hires.png)

##### Q-Q Plot

"Q" in *Q-Q plot* stands for *quantile*, as this plot compares empirical
and theoretical distribution (in this case, *normal* distribution) by
plotting their quantiles against each other. For normal distribution,
plotted dots should approximate a "straight", `x = y` line.

[![image](975387b3193e28fb08a85f37cb17f87e.png)](975387b3193e28fb08a85f37cb17f87e-hires.png)

##### Kernel Density Plot

*Kernel density plot* is a plot of smoothed *empirical distribution
function*. As such, it provides good insight about the shape of the
distribution. For normal distributions, it should resemble the well
known "bell shape".

[![image](1c20f2249107ddc2f8f5945197315e27.png)](1c20f2249107ddc2f8f5945197315e27-hires.png)

* * * * *

This report was generated with [R](http://www.r-project.org/) (2.14.0)
and [rapport](http://al3xa.github.com/rapport/) (0.2) in 6.843 sec on
x86\_64-unknown-linux-gnu platform.

![image](images/logo.png)