% Descriptives
% (Username not set) (E-mail address not set)
% 2011-04-26 20:25 CET

## Description

This template will return descriptive statistics of numerical, or
frequency tables of categorical variables.

### *gender* ("Gender")

The dataset has 709 observations with 709 valid values (missing: 0) in
*gender* ("Gender"). This variable seems to be a factor.

#### Base statistics

  **gender**   **N**     **pct**   **cum.n**   **cum.pct**
  ------------ --------- --------- ----------- -------------
  male         7344.00   60.93     7344.00     60.93
  female       4709.00   39.07     12053.00    100.00

#### Barplot

![image](2a42fb1eb44bf1361b44216c6b0c16ee.png)

It seems that the highest value is 2 which is exactly 2 times higher
than the smallest value (1).

### *age* ("Age")

The dataset has 709 observations with 709 valid values (missing: 0) in
*age* ("Age"). This variable seems to be numeric.

#### Base statistics

  **value**   **mean**   **sd**   **var**
  ----------- ---------- -------- ---------
  (all)       24.56      6.84     46.78

#### Histogram

![image](76fc57f9d2387aff730be60323f25624.png)

It seems that the highest value is 58 which is exactly 3.625 times
higher than the smallest value (16).

The standard deviation is 6.8399 (variance: 46.784). The expected value
is around 24.557, somewhere between 24.054 and 25.061 (SE: 0.2569).

If we suppose that *Age* is not near to a normal distribution (test: ,
skewness: 1.9568, kurtosis: 7.6428), checking the median (23) might be a
better option instead of the mean. The interquartile range (6) measures
the statistics dispersion of the variable (similar to standard
deviation) based on median.

## Description

This template will return descriptive statistics of numerical, or
frequency tables of categorical variables.

### *chatim* ("Chat & IM usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*chatim* ("Chat & IM usage"). This variable seems to be a factor.

#### Base statistics

  **chatim**    **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         896.00    9.03      896.00      9.03
  very rarely   1092.00   11.00     1988.00     20.03
  rarely        910.00    9.17      2898.00     29.20
  sometimes     1736.00   17.49     4634.00     46.69
  often         1988.00   20.03     6622.00     66.71
  very often    1316.00   13.26     7938.00     79.97
  always        1988.00   20.03     9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](18ee2d4410677e2bbc343a9a4889cc97.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *game* ("On-line games usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*game* ("On-line games usage"). This variable seems to be a factor.

#### Base statistics

  **game**      **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         5152.00   51.90     5152.00     51.90
  very rarely   1848.00   18.62     7000.00     70.52
  rarely        490.00    4.94      7490.00     75.46
  sometimes     910.00    9.17      8400.00     84.63
  often         532.00    5.36      8932.00     89.99
  very often    518.00    5.22      9450.00     95.20
  always        476.00    4.80      9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](db92f166fe1966dbd5c6f0b909c181b2.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *surf* ("Web surfing usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*surf* ("Web surfing usage"). This variable seems to be a factor.

#### Base statistics

  **surf**      **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         238.00    2.40      238.00      2.40
  very rarely   364.00    3.67      602.00      6.06
  rarely        476.00    4.80      1078.00     10.86
  sometimes     1624.00   16.36     2702.00     27.22
  often         2296.00   23.13     4998.00     50.35
  very often    2114.00   21.30     7112.00     71.65
  always        2814.00   28.35     9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](42a485477f7c7e629c55f3f106b2f482.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *email* ("Email usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*email* ("Email usage"). This variable seems to be a factor.

#### Base statistics

  **email**     **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         182.00    1.83      182.00      1.83
  very rarely   532.00    5.36      714.00      7.19
  rarely        714.00    7.19      1428.00     14.39
  sometimes     1260.00   12.69     2688.00     27.08
  often         1806.00   18.19     4494.00     45.28
  very often    1624.00   16.36     6118.00     61.64
  always        3808.00   38.36     9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](4271956be974e19ffa2034d316fd201c.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *download* ("Download usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*download* ("Download usage"). This variable seems to be a factor.

#### Base statistics

  **download**   **N**     **pct**   **cum.n**   **cum.pct**
  -------------- --------- --------- ----------- -------------
  never          154.00    1.55      154.00      1.55
  very rarely    406.00    4.09      560.00      5.64
  rarely         420.00    4.23      980.00      9.87
  sometimes      1190.00   11.99     2170.00     21.86
  often          1820.00   18.34     3990.00     40.20
  very often     2394.00   24.12     6384.00     64.32
  always         3542.00   35.68     9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](ec8a2289e719ec679a4abc2f1b3a62ec.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *forum* ("Web forums usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*forum* ("Web forums usage"). This variable seems to be a factor.

#### Base statistics

  **forum**     **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         1120.00   11.28     1120.00     11.28
  very rarely   1176.00   11.85     2296.00     23.13
  rarely        1036.00   10.44     3332.00     33.57
  sometimes     1736.00   17.49     5068.00     51.06
  often         1568.00   15.80     6636.00     66.85
  very often    1750.00   17.63     8386.00     84.49
  always        1540.00   15.51     9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](3f14c76d2ae5a41c21a771f3fd794ca3.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *socnet* ("Social networks usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*socnet* ("Social networks usage"). This variable seems to be a factor.

#### Base statistics

  **socnet**    **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         2940.00   29.62     2940.00     29.62
  very rarely   1554.00   15.66     4494.00     45.28
  rarely        826.00    8.32      5320.00     53.60
  sometimes     1316.00   13.26     6636.00     66.85
  often         1148.00   11.57     7784.00     78.42
  very often    1190.00   11.99     8974.00     90.41
  always        952.00    9.59      9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](c1a552be1b3a4299ff06e272129d8096.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *xxx* ("Adult sites usage")

The dataset has 709 observations with 709 valid values (missing: 0) in
*xxx* ("Adult sites usage"). This variable seems to be a factor.

#### Base statistics

  **xxx**       **N**     **pct**   **cum.n**   **cum.pct**
  ------------- --------- --------- ----------- -------------
  never         4102.00   41.33     4102.00     41.33
  very rarely   1792.00   18.05     5894.00     59.38
  rarely        770.00    7.76      6664.00     67.14
  sometimes     1918.00   19.32     8582.00     86.46
  often         672.00    6.77      9254.00     93.23
  very often    406.00    4.09      9660.00     97.32
  always        266.00    2.68      9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](053614b5b842759f559adcc0da8cc645.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).

### *long.use* ("How long you've been on the Internet?")

The dataset has 709 observations with 709 valid values (missing: 0) in
*long.use* ("How long you've been on the Internet?"). This variable
seems to be a factor.

#### Base statistics

  **long.use**         **N**     **pct**   **cum.n**   **cum.pct**
  -------------------- --------- --------- ----------- -------------
  less than 6 months   294.00    2.96      294.00      2.96
  1 years              728.00    7.33      1022.00     10.30
  2 years              966.00    9.73      1988.00     20.03
  3 years              1092.00   11.00     3080.00     31.03
  4 years              1064.00   10.72     4144.00     41.75
  5 years              1036.00   10.44     5180.00     52.19
  5 years and more     4746.00   47.81     9926.00     100.00

**Warning** in "if (is.numeric(var)) { ; rp.desc(NULL, rp.name(var),
c('mean', 'sd', 'var'), rp.data) ; } else { ; rp.freq(rp.name(var),
rp.data) ; }": "invalid factor level, NAs generated + invalid factor
level, NAs generated + invalid factor level, NAs generated"

#### Barplot

![image](ac7f8b3e1fb841eb17beaceee8e09dd1.png)

It seems that the highest value is 7 which is exactly 7 times higher
than the smallest value (1).