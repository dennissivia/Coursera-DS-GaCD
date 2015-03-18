# Coursera Getting and Cleaning Data (Coursera-DS-GaCD)

## Description
This project processes a raw data set containing human activity-recognition using smartphones.
The main script run_analysis.R downloads the raw data, cleans and filters it and creates a small and tidy dataset with the means per activity

The data, processes is available for download [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip). 

For futher details about the raw and generated data can be found in the [CookBook.md](CookBook.md)

## Usage

The script can simply be execute using R.
For example from a UNIX commandline:

```{r}
 R --vanilla < run_analysis.R
```

## Dependencies

The R package `reshape2` is required to run this script. This can be installed using
```{r}
install.packages("reshape2") 
```
