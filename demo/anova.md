% ANOVA Template
% Rapport package team @ https://github.com/aL3xa/rapport
% 2011-04-26 20:25 CET

## Description

An ANOVA report with table of descriptives, diagnostic tests and
ANOVA-specific statistics.

### Brief info

Two-Way ANOVA was carried out, with *Gender* and *Student* as
independent variables, and *Internet usage in leisure time (hours per
day)* as a response variable.

### Descriptives

The following table displays the descriptive statistics of ANOVA model.
You can see the factors on the left-hand side of the table, and summary
statistics on the right hand side.

  **gender**   **student**   **min(resp)**   **max(resp)**   **mean(resp)**   **SD(resp)**   **median(resp)**   **M.A.D.(resp)**   **skewness(resp)**   **kurtosis(resp)**   **min(Total)**   **max(Total)**   **mean(Total)**   **SD(Total)**   **median(Total)**   **M.A.D.(Total)**   **skewness(Total)**   **kurtosis(Total)**
  ------------ ------------- --------------- --------------- ---------------- -------------- ------------------ ------------------ -------------------- -------------------- ---------------- ---------------- ----------------- --------------- ------------------- ------------------- --------------------- ---------------------
  male         no            0.00            10.00           3.47             2.05           3.00               1.48               0.66                 2.81                 0.00             10.00            3.47              2.05            3.00                1.48                0.66                  2.81
  male         yes           0.00            12.00           3.17             1.94           3.00               1.48               1.37                 5.88                 0.00             12.00            3.17              1.94            3.00                1.48                1.37                  5.88
  male         Total         0.00            12.00           3.32             2.00           3.00               1.48               0.99                 4.07                 0.00             12.00            3.32              2.00            3.00                1.48                0.99                  4.07
  female       no            0.00            10.00           3.15             2.18           3.00               1.48               1.29                 4.59                 0.00             10.00            3.15              2.18            3.00                1.48                1.29                  4.59
  female       yes           0.00            12.00           3.01             2.43           2.00               1.48               1.44                 5.00                 0.00             12.00            3.01              2.43            2.00                1.48                1.44                  5.00
  female       Total         0.00            12.00           3.06             2.34           2.00               1.48               1.39                 4.90                 0.00             12.00            3.06              2.34            2.00                1.48                1.39                  4.90
  Total        Total         0.00            12.00           3.22             2.14           3.00               1.48               1.17                 4.51                 0.00             12.00            3.22              2.14            3.00                1.48                1.17                  4.51

**Warning** in "rp.desc(fac, resp, c(min, max, mean, SD = sd, median,
`M.A.D.` = mad, skewness, kurtosis), margins = TRUE)": "duplicated
levels will not be allowed in factors anymore"

### Diagnostics

Before we carry out ANOVA, we'd like to check some basic assumptions.
For those purposes, normality and homoscedascity tests are carried out
alongside several graphs that may help you with your decision on model's
goodness-of-fit.

#### Diagnostic tests

##### Normality tests

We will use *Shapiro-Wilk*, *Lilliefors* and *Anderson-Darling* tests to
screen departures from normalitty.

  -------- --------
  0.9385   0.0000
  0.1681   0.0000
  4.4600   0.0000
  0.8802   0.0000
  0.1721   0.0000
  3.4441   0.0000
  0.8872   0.0000
  0.1752   0.0000
  6.1519   0.0000
  0.8533   0.0000
  0.1819   0.0000
  7.3685   0.0000
  -------- --------

##### Homoscedascity tests

In order to test homoscedascity, *Bartlett* and *Fligner-Kileen* are
applied.

      **B**   **F**
  --- ------- -------
  D   10.72   3.40
  p   0.01    0.33

#### Diagnostic plots

Here you can see several diagnostic plots for ANOVA model.

### ANOVA table

### Off-topic stuff

input name: resp variable name: *leisure* variable label: *Internet
usage in leisure time (hours per day)* input label: *Response variable*
input description: *Dependent (response) variable*

input name: fac variable name: *gender* and *student* variable label:
*Gender* and *Student* input label: *Factor variables* input
description: *Independent variables (factors)*