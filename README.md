Getting and Cleaning Data Course 
Peer Assessment 

Description of how run_analysis.R script works.

1. Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.
2. Name the folder appropriately as 'tidydata'
3. Put folder "tidydata" and the R script(run_analysis.R) in the same working directory.
4. Source "run_analysis.R" (source("run_analysis.R")) using RStudio and run the script.
5. Look for two files:
    - merged_data.txt (7.95 Mb)
    - second_tidydata_w_average.txt (220 Kb)
6. Read the file using command  - tidyddata <- read.table("second_tidydata_w_average.txt.txt"). You should see 180 total rows.