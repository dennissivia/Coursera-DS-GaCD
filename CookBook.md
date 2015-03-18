# CookBook

# Input Data

The script creates a ./data subdirectory and downloads and extracts the [UCI dataset](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) into it. 

# Transformation and Output
According to the assessment requirements the following steps are taken to transform and summarize the data:

* Download the data and extract it
* load the `test`, `train` and `subject` datasets and merge them into one big dataset
* load the `features` and `activity_labels` files and merge them to obtain proper variable and activity naming 
* extract only the mean and standard deviation variables into a smaller subset
* create a tiny subset containing the mean of the smaller subset created, grouped by subject/activity
* save this data into `./data/tidy_data.txt`

The resulting subset for the mean calculation and the tidy dataset contain these variables. (see features_info.txt of the raw data archive)
<pre>
These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag
</pre>
The above variables where choosen as they included either mean or std in their original names.

