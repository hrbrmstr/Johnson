
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Johnson

Johnson transforms to normality using the Z family of distributions. It
performs the Johnson Transformation based on the method of the
percentiles. It includes the Anderson-Darling Test.

NOTE: This is a mod for a nigh-abandoned CRAN package to help answer
<https://stackoverflow.com/questions/47434667/r-ne-johnson-package-error-in-re-adtxsl-i-object-p-not-found>.

## Installation

You can install Johnson from github with:

``` r
# install.packages("devtools")
devtools::install_github("hrbrmstr/Johnson")
```

## The SO’s problem, resolved:

``` r
library(Johnson)

c(0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000,
0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000,
0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000, 0.0000000,
0.0000000, 0.4166667, 0.4166667, 0.4201681, 0.4201681, 0.4201681, 0.4219409,
0.4255319, 0.4255319, 0.4878049, 0.8333333, 0.8368201, 0.8403361, 0.8403361,
0.8438819, 1.2500000, 1.2500000, 1.2500000, 1.2605042, 1.2875536, 1.6666667,
1.6666667, 1.6666667, 1.6666667, 1.6666667, 1.6666667, 1.6736402, 1.6949153,
1.6949153, 1.6949153, 2.1186441, 2.1186441, 2.1186441, 2.5000000, 2.5000000,
2.5104603, 2.5210084, 2.5210084, 2.9166667, 2.9787234, 3.3333333, 3.3333333,
3.3898305, 3.3898305, 3.7500000, 3.7735849, 3.7974684, 4.1666667, 4.1841004,
4.6025105, 5.0000000, 5.0000000, 5.0847458, 5.0847458, 5.1724138, 5.3571429,
5.4621849, 5.5084746, 5.5555556, 6.6666667, 6.6666667, 6.7226891, 6.7796610,
6.7796610, 6.8965517, 7.0175439, 8.3333333, 8.3333333, 8.3333333, 8.3333333,
8.3333333, 8.3333333, 8.3333333, 8.3333333, 10.0000000, 0.0000000, 10.0000000,
10.1694915, 10.3448276, 11.2359551, 11.6666667, 2.2807018, 12.2881356,
13.5593220, 13.7931035, 13.7931035, 16.1016949, 6.2790698, 16.4556962,
16.9491525, 17.9487179, 26.1603376, 29.3103448, 2.2033898, 32.2033898,
32.2033898, 39.9159664) -> incorrectrecallpercent

str(RE.Johnson(incorrectrecallpercent))
#> List of 8
#>  $            : chr "Johnson Transformation"
#>  $ function   : chr "SB"
#>  $ p          : num 0.00058
#>  $ transformed: num [1:118] -1.08 -1.08 -1.08 -1.08 -1.08 ...
#>  $ f.gamma    : num 2.65
#>  $ f.lambda   : num 112
#>  $ f.epsilon  : num -0.921
#>  $ f.eta      : num 0.778
```
