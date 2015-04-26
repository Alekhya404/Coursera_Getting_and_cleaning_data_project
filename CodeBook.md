# Breif Description of the steps performed in the run_analysis.R script

Step 1: Merging Training and Test Data sets and creating one Data set
I have created 3 data sets Subject_data,Feature_data and Activity_data by combining the rows of training and test sets using rbind.
and then finally merged all the datasets together using "Cbind".Thus,finally create a "whole_data".


Step 2: Extracts only the measurements on the mean and standard deviation for each measurement. 
Here i had extracted the coloumns containing mean and standard deviations using "grep"and stored in mean_std_features.Then Subsetted
the desired coloumns in "Feature_data".

Step 3: Uses descriptive activity names to name the activities in the data set.
Extracted the names from activity_labels.txt using "read.table" and then updated the file using the names of this text file

Step 4: Appropriately labels the data set with descriptive variable names.
labeled the names of the "whole_data" using descriptive variable names

Step 5: From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Finally,generated a new dataset with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows). 
The output file is called tidy_data.txt, and uploaded to this repository.

# Variables Used
x_train,
