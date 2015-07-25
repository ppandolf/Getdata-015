##Usage reference for run_analysis.R  
 
This script computes mean and standard values on physical activity 
measurements determined using HAR (Human Activity Recognition) capabilities
of the Samsung Galaxy S smartphone 

##Source data URL:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

##A synopsis of the source data collection can be found here:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

A separate README.txt file within the source data zip package describes the 
physical actvity experiment and data collection methodology, and enumerates
the individual data files within the the zip package

## run_analysis.R Usage Notes

###Input 
run_analysis.R is written to read input files from the
/data/UCI HAR Dataset directory tree within the current R working directory.
Simply extract the entire "UCI HAR Dataset" folder from the source zip package
into a directory named "data" within the current R working directory, and verify
that the individual source files are located in applicable directories and subdirectories 
as follows:

	UCI HAR Dataset  
		activity_labels.txt
		features.txt 

        UCI HAR Dataset/train 
		X_train.txt
		y_train.txt
		subject_test.txt	
		
	UCI HAR Dataset/test folders and subfolders
		X_test.txt
		y_test.txt
		subject_test.txt				


###Process Steps To Produce Tidy Data
* extract, clean up, and apply data labels
* assemble test population data components
* assemble training population data components
* retain designated labeled variables for analysis
* integrate test and training data in common structure
* summarize variables (i.e. calculate group-column means) per assignment specification


###Final Output 
The tidy dataset file is written to the working directory /data subdirectory
and named getdata015_HARtidy.txt.  Please see CodeBook.md for tidy data element  
inventory.
    