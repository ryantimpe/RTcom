+++
# Date this page was created.
date = "2017-09-13"

# Project title.
title = "ipfitr"

# Project summary to display on homepage.
summary = "R package for expanding summary-level data to full detail using a variety of assumptions. [Github.io Page](https://ryantimpe.github.io/ipfitr/) |  [GitHub](https://github.com/ryantimpe/ipfitr) | [RMd Intro](../../files/Intro_to_ipfitr.html)"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "ipfitr.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["r", "packages"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

In market sizing and forecasting, we're often tasked with estimating large data tables with limited, high-level inputs. [Iterative proportion fitting](https://en.wikipedia.org/wiki/Iterative_proportional_fitting) has been used in market analysis for over 30 years. This package integrates the methodology, along with some more sophisticated methods, into the [tidyverse](https://github.com/tidyverse/tidyverse) in R.

The ipfitr package for R allows the user to input multiple high-level summary/aggregate data tables and create a single, full-dimension data table estimating individual cell values using iterative proportion fitting (IPFs).

The user can also submit must-hit target values or min/max conditions for individual cells or specific slices of the data table. 

Here's the link to a [webpage with a demo of key features](../../files/Intro_to_ipfitr.html). See my [GitHub](https://github.com/ryantimpe/ipfitr) for the script and latest updates. 


## Getting Started

The ipfitr package performs iterative proportion fitting on a seed datatable, continuously scaling values to each target until the seed values sum to every supplied target. If no seed is supplied, the function begins with a seed of 1 for every value. 

Changing the seed will result in different final results (see Examples 1a and 2 in [the demo](../../files/Intro_to_ipfitr.html)). For this reason, it's best to include as much information as you can about the relative values of the cells in the seed.

### Prerequisites

This package is built using the [tidyverse](https://github.com/tidyverse/tidyverse) packages. 

The functions in ipfitr can be run independently, but are more useful as part of a %>% workflow.

### Installing

``` r
install.packages(devtools)
devtools::install_github("ryantimpe", "ipfitr")
```

## Deployment

The Windows batch file RunDatasaur.bat is two lines telling Windows to run the R script using R 3.4. In future releases, this will be moved to AWS.

## Built With

* [R](https://www.r-project.org/) - R
* [tidyverse](https://github.com/tidyverse/tidyverse) - Tidyverse packages + ggplot2

## Versioning

For the versions available, see the [tags on this repository](https://github.com/ryantimpe/ipfitr/tags). 

## Authors

* **Ryan Timpe** - *Initial work* - [ryantimpe](https://github.com/ryantimpe)
* International Planning & Research - [iprcorp.com](https://iprcorp.com/)

See also the list of [contributors](https://github.com/ryantimpe/ipfitr/contributors) who participated in this project.

## License

No license.
