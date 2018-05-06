+++
# Date this page was created.
date = "2017-09-13"

# Project title.
title = "stats808 Box Office Modeling"

# Project summary to display on homepage.
summary = "Forecasting U.S. box office revenue with diffusion modeling. Updated version coming... eventually."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "stats808.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["analysis", "movies"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

[stats808.com](https://www.stats808.com) is a U.S. box office forecasting project I developed in 2014. While there are many econometric models available to forecast opening weekend, I went a step further by developing revenue forecasts for each week a movie is shown in theaters.

Using weekly U.S. box office data scraped from [Box Office Mojo](http://www.boxofficemojo.com/), consolidated review scores, and search engine activity using Google Trends, I developed models to forecast opening weekend revenue and total run revenue for new movies.

I then estimated weekday and weekend revenue for the remainder of each movie's run in theaters using [Bass diffusion models](https://en.wikipedia.org/wiki/Bass_diffusion_model) combined with theater count and film genre information.

These models were updated weekly with the release of revenue actuals for the previous week.

To [present the data](http://www.stats808.com/2014/08/weekly-forecast-august-8-2014/), I developed a WordPress post template with interactive D3.js charts and tables.

![stats808 example](../../img/stats808_weekly.jpg)

I will be revisiting this project in the future.