---
title: Pre-formatted files
weight: 10
draft: false
---


```r
require(quanteda)
require(readtext)
```

First, we show how to import pre-formatted files that come in a "spreadsheet format". `path_data` is the location of sample files on your computer that come with the **readtext** package.


```r
path_data <- system.file("extdata/", package = "readtext")
```

If your text data is stored in a pre-formatted file where one column contains the text and additional columns might store document-level variables (e.g. year, author, or language), you can use `read.csv()` to import.


```r
dat_inaug <- read.csv(paste0(path_data, "/csv/inaugCorpus.csv"))
```

Alternatively, you can use the **readtext** package to import character (comma- or tab-separated) values. **readtext** reads files containing text, along with any associated document-level variables.


```r
dat_inaug <- readtext(paste0(path_data, "/tsv/dailsample.tsv"), text_field = "speech")
```

{{% notice warning %}}
The most common problem in loading data into R is misspecifing locations of files or directories. If a path is relative, check where you are using `getwd()` and set the root directory of your project using `setwd()`. On Windows, you also have to replace all `\` in a path with `/`.
{{% /notice%}}

{{% notice tip %}}
If you have more than a few R files in a project, you should create a RStudio Project to better manage files and settings. You can create a RStudio project from the menu (_File > New Project_).
{{% /notice%}}
