# hurricane_harvey_labor - Event Study of Construction Labor Market Impacts

## What is this?

This repository contains the code, data processing pipeline, and LaTeX manuscript for a paper titled:

**“The Price of Disaster: Estimating the Impact of Hurricane Harvey on the Texas Construction Labor Market”**

The project uses county-level QCEW data to estimate the effect of Hurricane Harvey on wages and employment in the Texas construction sector, using an event-study difference-in-differences design.

## Prerequisites

Downloadable Data Needed: QCEW CSV Single Files 2016 - QCEW CSV Single Files 2019
https://www.bls.gov/cew/downloadable-data-files.htm

You will need the following installed:

- **R** (with the following packages):
  - `data.table`
  - `dplyr`
  - `ggplot2`
  - `fixest`
  - `tidyverse`

To install packages in R:
```r
install.packages(c("data.table", "dplyr", "ggplot2", "fixest", "tidyverse"))

## How to Run the Analysis

Prepare QCEW Data

Place the following files in the data/ directory:

2016.q1-q4.singlefile.csv

2017.q1-q4.singlefile.csv

2018.q1-q4.singlefile.csv

2019.q1-q4.singlefile.csv

Run the R Script

This script will:

Load and clean the QCEW data

Define treated and control groups

Create log-transformed employment and wage variables

Run an event-study difference-in-differences model

Generate two event study plots

Compile the Paper
