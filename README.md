# CNN_EEG_PD

### This is a CNN for PD Classification from Resting EEG

This repo contains the necessary data and code to replicate the findings from the manuscript: Generalizable electroencephalographic classification of Parkinson’s Disease using deep learning

preprocessed data can be accessed via zenodo: https://zenodo.org/record/8338680 

Add both folders to your drive, then you can run any of the five notebooks in this repo:

1. UNM_training - this will train a single replicate of the CNN and save the model so you can test it later. This model pertains to Table 1 in the manuscript. 
2. CV_UNM_no_leak - this will perform leave one subject out cross validation to accurately evaluate the model on the training data. This script generates the data for Figure 4 in the manuscript.
3. CV_UNM_with_leak - this will perform K-fold cross validation to estimate the accuracy on the training data. As per the manuscript, do not use for real testing. This script generates the data for figure 5 in the manuscript.
4. IU_testing_epoch_level - this will use the trained model on the testing data and report metrics after classifying each individual epoch of data. This script generates the data for Figure 6 and the first row of Table 3.
5. IU_testing_subject_level - this will use the trained model on the testing data and report metrics after classifying each subject. This script generates the data for Figure 7 and the second row of Table 3.

By default the notebooks will assume that you have the data folders "UNM_Data" and "Iowa_Data" in your drive. If you want to run the testing files without the training files, we have provided a demo file containing a model that you can load into the notebook. Do not change the demo's name and simply place it in your drive. All locations are up to you if you are willing to go into the notebooks and manually adjust their paths. 
