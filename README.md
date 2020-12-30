# Getting_and_Cleaning_Data_Final_Project
#1. get dataset from web
#Raw data was extracted from zip file and renamed dataDir
#2. merge {train, test} data set
#tables were created for each part of the data and were merged using the rbind function
#3. load feature & activity info
#feature and activity information was then added and combined with the rest of the data
#4. extract data by cols & using descriptive name
#allData$Activity and allData$Subject were the variable names used for extraction of data from the table created.
#5. generate tidy data set
#A new tidy dataset was produced using the write.table function

#This is the course project for the Getting and Cleaning Data Coursera course.
#The included R script, run_analysis.R, conducts the following:
#Download the dataset from web if it does not already exist in the working directory.
#Read both the train and test datasets and merge them into x(measurements), y(activity) and subject, respectively.
#Load the data(x's) feature, activity info and extract columns named 'mean'(-mean) and 'standard'(-std). Also, modify column names to descriptive. (-mean to Mean, -std to Std, and remove symbols like -, (, ))
#Extract data by selected columns(from step 3), and merge x, y(activity) and subject data. Also, replace y(activity) column to it's name by refering activity label (loaded step 3).
#Generate 'Tidy Dataset' that consists of the average (mean) of each variable for each subject and each activity. The result is shown in the file tidy_dataset.txt.
