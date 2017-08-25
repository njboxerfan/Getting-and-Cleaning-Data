# CodeBook

This is a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data.

## The datasets consist of the following files:

- 'features_info.txt': Shows information about the variables used on the feature vector.

- 'features.txt': List of all features.

- 'activity_labels.txt': Links the class labels with their activity name.

- 'train/X_train.txt': Training set.

- 'train/y_train.txt': Training labels.

- 'test/X_test.txt': Test set.

- 'test/y_test.txt': Test labels.

The following files are available for the train and test data. Their descriptions are equivalent.

- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.

- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_y_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis, respectively.

- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.

- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.

## The Variables

Only measurements on the mean and standard deviation were used from the original feature vector set. The signals used were:

- tBodyAcc-XYZ

- tGravityAcc-XYZ

- tBodyAccJerk-XYZ

- tBodyGyro-XYZ

- tBodyGyroJerk-XYZ

- tBodyAccMag

- tGravityAccMag

- tBodyAccJerkMag

- tBodyGyroMag

- tBodyGyroJerkMag

- fBodyAcc-XYZ

- fBodyAccJerk-XYZ

- fBodyGyro-XYZ

- fBodyAccMag

- fBodyBodyAccJerkMag

- fBodyBodyGyroMag

- fBodyBodyGyroJerkMag


## Transformation details

There are 6 parts:

1. Load the activity labels, data column names, and test and train data sets
2. Extract only the measurements on the mean and standard deviation for each measurement
3. Merge the training and the test sets to create one data set
4. Use descriptive activity names to name the activities in the data set
5. Appropriately label the data set with descriptive activity names
6. Create a second, independent tidy data set with the average of each variable for each activity and each subject
