This code book describes the variables, the data, and any transformations or work that was performed to clean up the data.

The data was collected from the accelerometers from the Samsung Galaxy S smartphone.

Data source: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

Full description: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Variables:
  - activity: 1 of 6: "WALKING", "WALKING_UPSTAIRS", "WALKING_DOWNSTAIRS", "SITTING", "STANDING", "LAYING"
  - subject: 1 of 30 integer identifying a subject
  - 66 other variables related to movement that contain 'mean' or 'std' in their name

There is no missing data.
The transformations on the data (documented in comments on the run_analysis.R script):
  - mergings of data from different files: train & test sets; vector of variables, label (activity) and subject id.
  - labeling column names.
  - subsetting: selection of variables that contain 'mean' or 'std' in their name.
  - grouping & summarising data