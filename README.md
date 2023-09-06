# Detecting Throat Cancer From Laryngitis from Patient Speech using Machine Learning

In this work we use machine learning to classify patients with throat cancer and laryngitis from their speech. We use recordings frm the Saarbruecken Voice Database (which can be found [here](https://www.stimmdatenbank.coli.uni-saarland.de/help_en.php4#menu)).

The code used in this work is split into three folders:

**FeatureExtraction** contains four notebooks which can be used to extract the five different feature sets (Wav2Vec2 feature states, Wav2Vec2 hidden states, Praat, openSMILE, and MFCCs). All feature extracted for both the test and train set are stored as csv files in the **_FeatureSets_** subfolder.

**Models** contains one notebook which can be used to create the SVM classifier using the feature sets. This folder also contains all of the models created during our experiments. 

**FeatureImportance** contains three notebooks _MakingModels_ calculates the feature importance of each feature and creates the models for each feature subset. _plottingImportance_ plots the balanced accuracy, precision, and recall of each of the models created in the _MakingModels_ notebook.
