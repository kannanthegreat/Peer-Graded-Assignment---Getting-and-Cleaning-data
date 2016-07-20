# Peer-Graded-Assignment---Getting-and-Cleaning-data
The purpose of this project is to demonstrate ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.


## Getting and cleaning data Course Project Peer Assignment
## Readme for run_analysis.R
        
        ### Purpose
        
## This script processes data from the Human Activity Recognition Using Smartphones Dataset to extract the average means and 
## standard  deviations of each variable for a given subject and activity, returning a tidy data frame containing these values.

## The script was prepared to meet the requirements of an assignment in the Getting and Cleaning Data Course offered on Coursera

        ### Source Data
        
        ## credit for the Human Activity Recognition Using Smartphones Dataset to:
        
        ## Jorge L. Reyes-Ortiz(1,2), Davide Anguita(1), Alessandro Ghio(1), Luca Oneto(1) and Xavier Parra(2)


        ## www.smartlab.ws

                ## Data available here:
                ## https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

                ## With a full description here:
        
        ## http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

        ### Assumptions
        
        ## The script assumes the data will be found in the directory "./UCI HAR Dataset/" structured as it is in the linked archive.
       

        ### Use
        ## The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. 
		## Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist
		## Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz
		## The experiments have been video-recorded to label the data manually 
		## The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 
		## 30% the test data 

## The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in 
## fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window)
## The sensor acceleration signal, which has gravitational and body motion components, was separated using a 
## Butterworth low-pass filter into body acceleration and gravity
## The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used
## From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details 

## For each record it is provided that


## - Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration
## - Triaxial Angular velocity from the gyroscope 
## - A 561-feature vector with time and frequency domain variables 
## - Its activity label 
## - An identifier of the subject who carried out the experiment

## The dataset includes the following files:


## - 'README.txt'

## - 'features_info.txt': Shows information about the variables used on the feature vector

## - 'features.txt': List of all features

## - 'activity_labels.txt': Links the class labels with their activity name

## - 'train/X_train.txt': Training set

## - 'train/y_train.txt': Training labels

## - 'test/X_test.txt': Test set

## - 'test/y_test.txt': Test labels
## run_analysis.R should do the following
## Merges the training and the test sets to create one data set
## Extracts only the measurements on the mean and standard deviation for each measurement
## Uses descriptive activity names to name the activities in the data set
## Appropriately labels the data set with descriptive variable names
## From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject

