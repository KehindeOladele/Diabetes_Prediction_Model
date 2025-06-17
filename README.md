# Diabetes_Prediction_Model

## Description
This is a machine learning model designed to predict the risk of diabetes based on health-related features such as; age, gender, race, smoking history, etc. This project leverages Random_Forest_Classifier to analyze patient data and predict potential diabetes risks.

## Features
•	Preprocessed <a href="diabetes_dataset.csv">dataset</a> for training.

•	Implementation of random_forest_classifier to create <a href="Diabetes_Prediction_Model.ipynb">model</a>.

•	Evaluation of Accuracy.

•	Implementation of a confusion metrics to check for precision and recall.

## Dataset
The dataset s a Comprehensive Clinical Dataset (100k rows) found in Kaggle. It initially had 16 columns namely: year, gender, age, location, race:AfricanAmerican, race:Asian, race:Caucasian, race:Hispanic, race:Other, hypertension, heart_disease, smoking_history, bmi, hbA1c_level, blood_glucose_level, diabetes; and 100,000 rows. The data types were initially float64(3), int64(10), object(3).
However, after exploring the dataset by using a correlaton metrics and some column charts, I chose to drop the year colummn. Using One_hot_encoding method, I split the gender and smoking history columns into different columns for the individual values giving either 0 for No or 1 for Yes. That done, I performed over-sampling on the data because the dataset was not balanced, only having 9% of the samples with diabetes. The ove-sampling was done using SMOTE (k-neighbors = 5).
Finally i stndardized the dataset.

## Model Training
The model training was done using Rando Forest Algorithm. The dataset was split into train and test data at the ratio 80:20 (test size = 0.2).

## Results
The model proved to be 96% acccurate with a recall of 92%  and a precision of 69%.

## Acknowledgments
The dataset was created by Priyam Choksi and was downloaded from Kaggle.
