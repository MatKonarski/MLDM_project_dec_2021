# MLDM_project

This repository consists of a participation inside “Rainforest Connection Species Audio Detection” Kaggle competition.
It consists of one notebook “Rainforest.ipynb” and one zip file with datasets furnished inside the Kaggle contest.

You can find description of the data here: https://www.kaggle.com/c/rfcx-species-audio-detection/data
One important point is that true positive and false positive are only considering one species during one period of the recording. You can have a false positive extract inside one recording but still earing the species at another moment.

The notebook consists of several parts:
-Work with one song where I load one recording, listen to audio and try basic process on the recording.
-Prediction on one species where I build one model for predicting if one extract is a true positive or a false positive for the species with the id 0. It consists of all the process that will be used during the training.
-Prediction on a full recording where I used the previously trained model in order to predict if we ear the species at any moment of a recording.
-Prediction on full test set for all species, using the previous process I am able to train one model by species and looked if we can ear that species inside the different recordings, I am saving this results for submission into Kaggle competition.

Kaggle score: 0.385
Max score: 0.612 score obtained without doing the filtering
