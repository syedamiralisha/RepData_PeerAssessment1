title: "Reproducible Research: Peer Assessment 1"
output: 
  html_document:
    keep_md: true
---

# Reproducible Research - Course Project 1

This document analyzes an activity dataset containing number of steps recorded in 5-minute intervals across various days.

It was generated using [Knitr](https://github.com/yihui/knitr)

	install.packages('knitr', dependencies = TRUE)
	library(knitr)
	knit2html("PA1_template.Rmd", force_v1 = TRUE)

It also includes some sample data output to verify results.


	
## Loading and preprocessing the data

The following code loads the data into a variable `activity`. The script will attempt to download and unzip the file if it doesn't exist inside the work directory.


```r
# Download zip file if it doesn't already exist in the workspace
dataurl <- "https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip"
if (!file.exists("activity.zip")) {
	download.file(dataurl, destfile = "activity.zip", method = "curl")
}
