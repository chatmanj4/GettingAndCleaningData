run_analysis.R performs the following:

1.Merges the training and test sets (train/X_train.txt with test/X_test.txt), yielding a 10299x561 data frame, then train/subject_train.txt with test/subject_test.txt, yielding a 10299x1 data frame with subject IDs, and train/y_train.txt with test/y_test.txt, yielding a 10299x1 data frame with activity IDs.

2.Reads features.txt and extracts the measurements with the mean and standard deviation for each measurement. This yields  a 10299x66 data frame.

3.Reads activity_labels.txt and applies descriptive activity names to the activities in the data set(walking, walkingupstairs, walkingdownstairs, sitting, standing, laying)

4.The script labels the data set with descriptive names: all feature names (attributes) and activity names are converted to lower case, underscores and brackets () are removed. It is then saved in the mergeddata.text file.  

5.Finally, the script creates a 2nd, independent tidy data set with the average of each measurement for each activity and each subject. The result is saved as tidyWithAverages.txt, a 180x68 data frame with the following names:

[1] "subject"
[2] "activity"
[3] "tBodyAcc-mean()-X"
[4] "tBodyAcc-mean()-Y"
[5] "tBodyAcc-mean()-Z"
[6] "tGravityAcc-mean()-X"
[7] "tGravityAcc-mean()-Y"
[8] "tGravityAcc-mean()-Z"
[9] "tBodyAccJerk-mean()-X"
[10] "tBodyAccJerk-mean()-Y"
[11] "tBodyAccJerk-mean()-Z"
[12] "tBodyGyro-mean()-X"
[13] "tBodyGyro-mean()-Y"
[14] "tBodyGyro-mean()-Z"
[15] "tBodyGyroJerk-mean()-X"
[16] "tBodyGyroJerk-mean()-Y"
[17] "tBodyGyroJerk-mean()-Z"
[18] "tBodyAccMag-mean()"
[19] "tGravityAccMag-mean()"
[20] "tBodyAccJerkMag-mean()"
[21] "tBodyGyroMag-mean()"
[22] "tBodyGyroJerkMag-mean()"
[23] "fBodyAcc-mean()-X"
[24] "fBodyAcc-mean()-Y"
[25] "fBodyAcc-mean()-Z"
[26] "fBodyAcc-meanFreq()-X"
[27] "fBodyAcc-meanFreq()-Y"
[28] "fBodyAcc-meanFreq()-Z"
[29] "fBodyAccJerk-mean()-X"
[30] "fBodyAccJerk-mean()-Y"
[31] "fBodyAccJerk-mean()-Z"
[32] "fBodyAccJerk-meanFreq()-X"
[33] "fBodyAccJerk-meanFreq()-Y"
[34] "fBodyAccJerk-meanFreq()-Z"
[35] "fBodyGyro-mean()-X"
[36] "fBodyGyro-mean()-Y"
[37] "fBodyGyro-mean()-Z"
[38] "fBodyGyro-meanFreq()-X"
[39] "fBodyGyro-meanFreq()-Y"
[40] "fBodyGyro-meanFreq()-Z"
[41] "fBodyAccMag-mean()"
[42] "fBodyAccMag-meanFreq()"
[43] "fBodyBodyAccJerkMag-mean()"
[44] "fBodyBodyAccJerkMag-meanFreq()" [45] "fBodyBodyGyroMag-mean()"
[46] "fBodyBodyGyroMag-meanFreq()"
[47] "fBodyBodyGyroJerkMag-mean()"
[48] "fBodyBodyGyroJerkMag-meanFreq()"
