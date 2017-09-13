
<!-- README.md is generated from README.Rmd. Please edit that file -->
Overview
--------

Constellation contains a set of functions for applying multidimensional, time window based logic to time series data frames of arbitrary length. Constellation was developed to enable rapid and flexible identification of series of events that occur in hospitalized patients. The functions have been abstracted for general purpose use with time series data. Constellation extends and provides a friendly API to rolling joins and overlap joins implemented in [data.table](https://cran.r-project.org/web/packages/data.table/data.table.pdf).

There are three functions included in constellation to build complex features from time series data:

-   `value_change()` identify increases or decreases in a value within a given time window
-   `constellate()` identify time stamps when a series of events occur within a given time window
-   `constellate_criteria()` identify which events occur within a given time window for every measurement time stamp

Constellation can be used to build point-based scores for time series data, identify particular sequences of events that occur near each other, and identify when specific changes occur for a given parameter.

If you are new to constellation, the best place to start is the `vignette("constellation", "identify_sepsis")`.

Installation
------------

You can install constellation from github with:

``` r
# install.packages("devtools")
devtools::install_github("marksendak/constellation")
```

This package is under development in preparation of release on CRAN. If you have any questions, comments, or feedback, please email <mark.sendak@gmail.com>.

Example
-------

This is a basic example which shows you how to solve a common problem:

``` r
## basic example code
```

Why constellation?
------------------

In clinical medicine, there are a subset of conditions that are defined by a sequence of related events that unfold over time. These conditions are described as a "*constellation of signs and symptoms*."

Duke Institute for Health Innovation
------------------------------------

constellation was originally developed to support a machine learning project at the [Duke Institute for Health Innovation](http://www.dihi.org/) to predict sepsis.