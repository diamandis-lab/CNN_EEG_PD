# CNN_EEG_PD

### This is a CNN for PD Classification from Resting EEG

This repo contains the necessary data and code to replicate the findings from the manuscript: Generalizable electroencephalographic classification of Parkinson’s Disease using deep learning

Preprocessed UNM data can be accessed via google drive here: https://drive.google.com/drive/folders/1kKqpM21GQVYue-owZ7dQuwDnCw8uQktd?usp=sharing
Preprocessed UIowa data can be accesed via google drive here: https://drive.google.com/drive/folders/19QJgQCEP-09rx_O4ItiBybzLjfKaPNxF?usp=sharing

Add both folders to your drive, then you can run any of the five scripts in this repo:

1. UNM_training - this will train a single replicate of the CNN and save the model so you can test it later.
2. CV_UNM_no_leak - this will perform leave one subject out cross validation to accurately evaluate the model on the training data.
3. CV_UNM_with_leak - this will perform K-fold cross validation to estimate the accuracy on the training data. As per the manuscript, do not use for real testing.
4. IU_testing_epoch_level - this will use the trained model on the testing data and report metrics after classifying each individual epoch of data.
5. IU_testing_subject_level - this will use the trained model on the testing data and report metrics after classifying each subject. 


