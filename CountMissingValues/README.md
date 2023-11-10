
<!-- README.md is generated from README.Rmd. Please edit that file -->

# CountMissingValues

<!-- badges: start -->
<!-- badges: end -->

The goal of CountMissingValues is to give count_all_missing_by_group a
data frame and column group, which will return a table containing the
levels of group in the first column, and number of missing values for
each given column in subsequent columns.

## Installation

You can install the development version of CountMissingValues like so:

``` r
# library(devtools)

devtools::install_github("stat545ubc-2023/BaseEditor-CountMissingValues")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(CountMissingValues)
count_all_missing_by_group(airquality, Month)
#> # A tibble: 5 × 6
#>   Month Ozone Solar.R  Wind  Temp   Day
#>   <int> <int>   <int> <int> <int> <int>
#> 1     5     5       4     0     0     0
#> 2     6    21       0     0     0     0
#> 3     7     5       0     0     0     0
#> 4     8     5       3     0     0     0
#> 5     9     1       0     0     0     0
```
