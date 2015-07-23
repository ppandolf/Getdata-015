##Usage reference for run_analysis.R  
 
This script computes mean and standard values on physical activity 
measurements captured on the Samsung Galaxy S smartphone

###Source data URL:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip


###Usage Notes
A separate README.txt file within the source data zip package describes the 
physical actvity experiment and data collection methodology, and enumerates
the individual data files within the the zip package
of the experimentset   
 
please see CodeBook.md for details about the data extraction and manipulation
performed by run_analysis.R

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


###Final Output 
The tidy dataset file is written to the working directory /data subdirectory
and named getdata015_HARtidy.txt 
    