GettingAndCleaningData
======================

1.Unzip the source (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) into a folder on your local drive

2.Put run_analysis.R into desired location

3.In RStudio set working directory to the location of your run_analysis.R file

4.Use data <- read.table("data_set_with_the_averages.txt") to read the data. 


The R script called run_analysis.R

1. Merges the training and the test sets to create one data set.

2. Extracts only the measurements on the mean and standard deviation for each measurement. 

3. Uses descriptive activity names to name the activities in the data set

4. Appropriately labels the data set with descriptive activity names. 

5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

Processing performed by run_analysis.R script:

Part 1

1.Read data from raw files and convert them to the proper types

2.Merge the training and test data sets

3.Save the data set to a csv file with a txt extension

Part 2

1.Read in data from part 1

2.Process data and perform averages and labeling 

3.Save the new dataset to a csv file with a txt extension

