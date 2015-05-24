Getting and Cleaning Data Course
Peer Assessment

Below is the description of the variables, the data, and any transformations or work that I have performed to clean up the data in use.

A full description is available at the site where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Below is the link to the data for the project:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Below is what run_analysis.R script does to clean up the data:
    1. Read X_train.txt, y_train.txt and subject_train.txt (from the "./tidydata/train" folder)
    2. Saves them in trainTinyData, trainLabel and trainSubject variables respectively.
    3. Read X_test.txt, y_test.txt and subject_test.txt from the "./tidydata/test" folder 
    4. Saves them in testTidyData, testLabel and testsubject variables respectively.
    5. Used joinData to concatenate testTidyData to trainTidyData
    6. Used joinLabel to concatenate testLabel to trainLabel
    7. Used joinSubject to concatenate testSubject to trainSubject
    8. Read features.txt file from the "/tidydata" folder and store the data in a features variable.
    9. Clean the column names of the subset. "()" and "-" are removed from names
    10. Capitalize "M" and "S" in "Mean" and "std"
    11. Read activity_labels.txt file from "/tidydata" folder and store the data in a activity variable.
    12. Clean the activity names. Change all names to lower cases. 
    13. Remove underscore between letters and Capitalize the first letter after.
    14. Transform the values of joinLabel
    15. To get cleaned data frame Combine the joinSubject, joinLabel and joinData by column.    
    16. Appropriately label "subject" and "activity" for the first columns. 
    17. Write the result out to "merged_data.txt" file in current working directory.
    18. Create a second,independent tidy data set with the average of each variable for each activity and each subject. Named the result file "second_tidydata_w_average.txt""
