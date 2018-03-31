
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Travis build
status](https://travis-ci.org/ijlyttle/altair.svg?branch=master)](https://travis-ci.org/ijlyttle/altair)
[![CRAN
status](https://www.r-pkg.org/badges/version/altair)](https://cran.r-project.org/package=altair)

# altair

The goal of altair is to provide an interface to the
[Altair](https://altair-viz.github.io) Python package, which builds
Vega-Lite visualizations. This is a short term solution - I am a big fan
of the native R interface to build Vega-Lite visualizations that Bob
Rudis (@hrbrmstr) and coworkers are building with the
[vegalite](https://vega.github.io/vega-lite) package.

## Development plan

For the foreseeable future, this package is going to be very rough. At
the moment, you are able to muck around with Vega-Lite 2.0. This means:

1.  You can create charts by accessing the Python **Altair** API using
    **reticulate**.
2.  You can display charts using the `vegalite()` htmlwidget.

There’s really not much beyond that. Here’s what I have in mind for the
near future:

1.  Tooltips.
2.  A proper installation procedure for the Altair Python package, a
    function like `install_altair()`.

In the longer-term future it may be interesting to provide a proper R
interface to the Python API. I have no idea what that looks like,
although we might take some inspiration from the
[keras](https://keras.rstudio.com/) package.

## Installation

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("ijlyttle/altair")
```

## Acknowledgements

This package does not contribute much new; it rests on these
foundations:

  - [Altair](https://altair-viz.github.io): Python interface to
    Vega-Lite
  - [Reticulate](https://rstudio.github.io/reticulate): R framework to
    work with Python
  - [Vega-Lite](https://vega.github.io/vega-lite): A grammar of
    interactive graphics
  - [D3](https://d3js.org): Data-driven documents
  - [vegalite](https://github.com/hrbrmstr/vegalite): Native R interface
    to Vega-Lite

## Code of conduct

Please note that this project is released with a [Contributor Code of
Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree
to abide by its terms.
