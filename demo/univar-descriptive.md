% Descriptives
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

## Description

This template will return descriptive statistics of a numerical, or a
frequency table of a categorical variable.

### *gender* ("Gender")

The dataset has 709 observations with 673 valid values (missing: 36) in
*gender* ("Gender"). This variable seems to be a factor.

#### Base statistics

          **gender**   **N**    **pct**   **cumul.count**   **cumul.pct**
  ------- ------------ -------- --------- ----------------- ---------------
  1       male         410.00   60.92     410.00            60.92
  2       female       263.00   39.08     673.00            100.00
  Total                673.00   100.00    673.00            100.00

#### Barplot

![image](3ed92ab3ffc6e875335e7e8c774c35a8.png)

It seems that the highest value is 2 which is exactly 2 times higher
than the smallest value (1).

## Description

This template will return descriptive statistics of a numerical, or a
frequency table of a categorical variable.

### *age* ("Age")

The dataset has 709 observations with 677 valid values (missing: 32) in
*age* ("Age"). This variable seems to be numeric.

#### Base statistics

  **value**   **mean(age)**   **sd(age)**   **var(age)**
  ----------- --------------- ------------- --------------
  (all)       24.57           6.85          46.91

#### Histogram

![image](ac5d789145bdef09b10219ef16429f53.png)

It seems that the highest value is 58 which is exactly 3.625 times
higher than the smallest value (16).

The standard deviation is 6.8491 (variance: 46.911). The expected value
is around 24.573, somewhere between 24.057 and 25.089 (SE: 0.2632).

If we suppose that *Age* is not near to a normal distribution (test: ,
skewness: 1.9296, kurtosis: 7.4851), checking the median (23) might be a
better option instead of the mean. The interquartile range (6) measures
the statistics dispersion of the variable (similar to standard
deviation) based on median.