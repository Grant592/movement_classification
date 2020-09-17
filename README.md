# Human Movement Classification

Human movement classification using smartphone and smartwatch data from [WISDM Dataset](https://archive.ics.uci.edu/ml/datasets/WISDM+Smartphone+and+Smartwatch+Activity+and+Biometrics+Dataset+).

## Notes
* [movement_classification.ipynb](movement_classification.ipynb) is messy and won't run in order. This was an experiment of various techniques including clustering (KNN and T-SNE), XGBoost and neural networks; both standard dense networks and using RNNs.
*  [movement_classification_cleaned.ipynb](movement_classification_cleaned.ipynb) is a tidier version only containing attempts at classification using tensorflow models.

## Summary
The most successful model at 77% accuracy used the data from the watch accel and gyro data using a period of 200 samples (i.e. a 10 second period) and a stride of 200 (i.e. no overlap between the samples).  The main classes that were classified incorrectly were the various eating classes which looked quite erratic when graphed

## To-do
* Remove the eating classes and see if accuracy can be imporved on the more movement based tasks alone


