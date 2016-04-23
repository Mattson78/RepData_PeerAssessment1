---
title: 'Reproducible Research: Peer Assessment 1'
author: "Mattson78"
date: "23 april 2016"
output: word_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## 



```{r, echo=TRUE}
if(!file.exists("activity.csv")){
  unzip("activity.zip")
}
activityData <- read.csv("activity.csv")

```

## 

You can also embed plots, for example:

```{r, echo=TRUE}
qplot(stepsByDay, xlab = "Total Steps by Day", ylab = "frequency using binwith 600", binwidth = 600)
```

Note that the `echo = TRUE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
