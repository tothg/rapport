% Descriptive statistics
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

Description
-----------

This template will return descriptive statistics of numerical or
frequency tables of categorical variables.

*2*

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

![image](3ed92ab3ffc6e875335e7e8c774c35a8.png)

It seems that the highest value is *2* which is exactly 2 times higher
than the smallest value (*1*).

The most frequent value is *male*.

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

![image](bde5b5e4ca06fa103953fc17e5273291.png)

Description
-----------

This template will return descriptive statistics of numerical or
frequency tables of categorical variables.

*8*

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

![image](5a00abbe4c793ceedbbf10939665b5cf.png)

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

![image](e53046a09491443064e085131e547971.png)

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

![image](0166a8b5df2f3db871e8736bfee8af6e.png)

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

![image](895cde198b269bf65b01e1e067a515c8.png)

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

![image](dde181184885b8777d0248b3f421289a.png)

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

![image](ac419134b2f4695e544d8886ba12e0c2.png)

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

![image](8475d98870c1cdd2436a3abdb0d69a66.png)

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

![image](4fda8cf992e8de93624c45ef3c72a0c5.png)

It seems that the highest value is *7* which is exactly 7 times higher
than the smallest value (*1*).

The most frequent value is *never*.

Description
-----------

This template will return descriptive statistics of numerical or
frequency tables of categorical variables.

*2*

*hp*
----

The dataset has *32* observations with *32* valid values (missing: *0*)
in *hp*, which seems to be a quantitative variable.

### Base statistics

  **value**   **mean(hp)**   **sd(hp)**   **var(hp)**
  ----------- -------------- ------------ -------------
  (all)       146.6875       68.5629      4700.8669

### Histogram

![image](d90ec4a0af55fabeae7988710a062ce0.png)

It seems that the highest value is *335* which is exactly 6.4423 times
higher than the smallest value (*52*).

The standard deviation is *68.5629* (variance: *4700.8669*). The
expected value is around *146.6875*, somewhere between *122.9317* and
*170.4433* with the standard error of *12.1203*.

If we suppose that *hp* is not near to a normal distribution (test: see
below, skewness: *0.7614*, kurtosis: *3.0522*), checking the median
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

![image](d90ec4a0af55fabeae7988710a062ce0.png)

##### Q-Q Plot

"Q" in *Q-Q plot* stands for *quantile*, as this plot compares empirical
and theoretical distribution (in this case, *normal* distribution) by
plotting their quantiles against each other. For normal distribution,
plotted dots should approximate a "straight", `x = y` line.

![image](17e5c77b83c6e3e636487406decc14c7.png)

##### Kernel Density Plot

*Kernel density plot* is a plot of smoothed *empirical distribution
function*. As such, it provides good insight about the shape of the
distribution. For normal distributions, it should resemble the well
known "bell shape".

![image](e63199776da0ad4146eff538e5ef7af7.png)

*wt*
----

The dataset has *32* observations with *32* valid values (missing: *0*)
in *wt*, which seems to be a quantitative variable.

### Base statistics

  **value**   **mean(wt)**   **sd(wt)**   **var(wt)**
  ----------- -------------- ------------ -------------
  (all)       3.2172         0.9785       0.9574

### Histogram

![image](10caa8222b28328a6d8fd28917cbfb45.png)

It seems that the highest value is *5.424* which is exactly 3.5849 times
higher than the smallest value (*1.513*).

The standard deviation is *0.9785* (variance: *0.9574*). The expected
value is around *3.2172*, somewhere between *2.8782* and *3.5563* with
the standard error of *0.173*.

If we suppose that *wt* is not near to a normal distribution (test: see
below, skewness: *0.4438*, kurtosis: *3.1725*), checking the median
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

![image](10caa8222b28328a6d8fd28917cbfb45.png)

##### Q-Q Plot

"Q" in *Q-Q plot* stands for *quantile*, as this plot compares empirical
and theoretical distribution (in this case, *normal* distribution) by
plotting their quantiles against each other. For normal distribution,
plotted dots should approximate a "straight", `x = y` line.

![image](ff471a5bcb80aaf91b4c053ab038d69a.png)

##### Kernel Density Plot

*Kernel density plot* is a plot of smoothed *empirical distribution
function*. As such, it provides good insight about the shape of the
distribution. For normal distributions, it should resemble the well
known "bell shape".

![image](c3769779837adedcb4198ec881cc946b.png)

* * * * *

This report was generated in [R](http://www.r-project.org/) with
[Rapport](http://al3xa.github.com/rapport/) in 3.061 sec. Feel free to
create [your own reporting
templates](http://al3xa.github.com/rapport/#custom)!

![image](images/rapport.png)