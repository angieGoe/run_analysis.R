Project run_analysis.R Function
==============

This files contains how the scrips of this repo work. 
The R Script `run_analysis.R` can download and process the required data. It does the following: 

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement. 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names. 
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

The new Tidy data sets are: 
- `data_set.txt` : combines training and test data sets (together with subject and activity data).

- `average_vbles.txt` : aggregates the aforementioned data by subject and activity (the mean of multiple trials for each feature is taken).

## Source

Information about used data in: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Used data set: [zip file](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) 
(NOTE: the R script created will download it from the source if necessary).


====================
## Dependencies

`run_analysis.R` depends on `reshape2` and `plyr` libraries 
(NOTE: The R script created will install and load them if necessary).

