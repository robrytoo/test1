# CodeBook Introduction

This codebook has three sections.  

* VARIABLES describes the columns in the output file >tidyStep5.txt that results from running >run_analysis.R on the data set downloaded from the UCI Machine Learning Repository at
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

* DATA explains the data from the repository that is used as input to the “run_analysis.R” file.

* TRANSFORMATIONS explains calculations necessary to transform DATA to the VARIABLES



## VARIABLES

The output file “tidyStep5.txt” contains a data frame of 180 rows by 88 columns.  Each of the column from the source dataset that represents a mean or standard deviation of a training/testing set variable (i.e. contains the strings “STD” or “mean” (case insensitive)) is retained to yield 86 columns.  Each row is column is the mean of the retained variable for  

## DATA

The original downloaded used for input to the “run_analysis.R” file  consists eight files.  

Feature files
- X_train.txt  (7352 observations of 561 features)
- X_test.txt (2947 observations of 561 features)
These features were derived from the raw data collected by the Samsung accelerometers  (see the web site file          ) and each observation corresponds to a derived feature for an individual subject engaged in a single activity.  The files 
	- y_train.txt (7352 coded activities (categorical values 1 to 6)) 	
      - y_test.txt (2947 coded activities (categorical values 1 to 6))
indicate the activity for each observation and the files
	- subject_train.txt (7352 coded subjects (categorical values 1 to 30))
	- subject_test.txt (2947 coded subjects (categorical values 1 to 30)) 
The file 
	- features.txt 
indicates the name of the 561 feature in training and testing feature files.
The file 
	- activity_labels.txt 
defines the six categorical coded activities. 
       
