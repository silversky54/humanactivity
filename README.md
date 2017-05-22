Getting and cleaning data course Project

This project is part of coursera Getting and clieaning data course. 
The main objective of this project is to read data from the "Human Activity Recognition  Analysis", reshape the data as necessary to make it tidy
and write a new data sat that has the averages of the "mean" and "std" features descrived in the original data. 

This Repo includes the following files
README.txt: Readme text file with a description of the project and files included
run_analysis.R: R script which reads Test and Training data from a Human Activity Recognition anlysis and experiment, reshapes it and produces a tidy summarized dataset 
summ_activity_avg.txt: the summary dataset that is the result of running run_analysis.R
summ_dataset_info.md: code book of the data and variables included in the summ_activity_avg.txt dataset

run_analysis.R follows the following general process:
It reads the original Human Activiy Datasets for Test and Training which are each split into 3 files: 
1. A 561-feature vector with time and frequency domain variables. 
2. Its activity label. 
3. An identifier of the subject who carried out the experiment.

In the script then combines all 3 datasets and then merges the Test and Training data sets. From this new dataset we select the variables that represent a mean or standard deviation and reshape the dataset to convert the feature columns which combine feature and variable data into a new tidy dataset.
Then we we calculate the average of the mean and std variables per subject, activity and feature. The result is stored in a new dataset named "summ_activity_avg.txt".

This scrip requires The Human Activity Recognition Dataset which can be downloaded from the following site including its description:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip