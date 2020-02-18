# Getting-and-Cleaning-Data-Final-Project

This repo contains a README.rtf file, also copy/pasted below.  This briefly explains my project.  Details about how I made my R script and, ultimately, my data frames, are given in the R script itself as it takes the viewer through step-by-step.  Included also in this repo is a codebook explaining the variables used in my data frames.  Here is the README rtf text:

This information comes from a study originally done in 2012 by Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, and Luca Oneto at SmarLab.  It takes data from SmartPhones that help to the scientists to study body movements in relation to Health apps: what does it look like when people sit, stand, walk upstairs, walk downstairs, walk on level ground or lay down.  The original study looks at time and frequency statistics that include 3-D angle measurements, body accelerations and gravity pulls.  Information about the original project and studies can be found at http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones (description) and https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip (data).  A codebook with variable names is also a part of this repo.  The original experiment, off of which my work is based, took 30 people and visually measured the above variables.  70% of the data was designated as training data and 30% as testing data (randomly decided).

My repo contains this README, and the codebook mentioned above and the R script to do replicate the work that I did.  The R script gives detailed instructions and explanations as it walks you through step-by-step what is going on.

I combined the test and training data into one giant data frame.  I then extracted only the variables (columns) that discussed means and standard deviations.  The means and standard deviations included body acceleration and jerk along 3 axes (3-dimensional), gravity acceleration and jerk and angular velocity in 3-D, and all of this was calculated with both time and frequency variables, for a total of 79 extracted variables in the data frame.  There were a total of 10,299 observations on these variables.  The R script detailing all of this is called run_analysis.R.

After creating this data frame, I created one more small data frame that consisted of the mean values for each of the 79 aforementioned variables.  