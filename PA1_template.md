# Reproducible Research: Peer Assessment 1

Unzip activity.zip gives activity.csv

## Loading and preprocessing the data

```r
data<-read.csv("activity.csv")
```
After reading activity.csv we check dimensions of data. Two months together have 17,568 observals, the intervals of 5 minutes (= 30+31 days\*24 hours\*(60 minutes/5 minutes). There are three variables: total steps, date and interval

```r
dim(data)
```

```
## [1] 17568     3
```
Let's take a look at first five rows:

```r
head(data)
```

```
##   steps       date interval
## 1    NA 2012-10-01        0
## 2    NA 2012-10-01        5
## 3    NA 2012-10-01       10
## 4    NA 2012-10-01       15
## 5    NA 2012-10-01       20
## 6    NA 2012-10-01       25
```
The column with steps measurements are steps. There are missing observations.

```r
steps<-data$steps
summary(steps)
```

```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max.    NA's 
##     0.0     0.0     0.0    37.4    12.0   806.0    2304
```
What is impact of missing data on steps?

```r
mean(is.na(steps))
```

```
## [1] 0.1311
```
Approx 13% of data steps is missing. For now these can be ingored



## What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
