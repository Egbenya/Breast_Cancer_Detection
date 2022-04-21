Breast Cancer Detection

Datasets: "https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/breast-cancer-wisconsin.data"

Overview

Objective 1: Train a KNN algorithm to detect breast cancer.

I imported the necessary libraries

I Imported the breast-cancer-wisconsin.data datasets from their website , and assigned them to data_df.

I Performed some data exploration on the dataset for clarity purposes.

I identified and deleted duplicates values.

I identified the missing value ('?') in the “bare_nuclei” column, since the missing values was about 2% of the entire data, I deleted the rows with missing values.

I deleted the id columns from the DataFrame. It was non significant to our prediction.

I visualise my DataFrame using matplotlib hist, seaborn countplot, and pandas scatter_matrix to gain better insight on the data

I split the data into features and response then labelled them X and y respectively.

I used train_test_split to split the data into training and test set with test_size=.20 and random_state=42

I scaled the X_train and X_test dataset using MinMaxScaler() in other to normalised the DataFrame.

I used the KNeighborsClassifier to instantiate a model on the normalised training data, %timed the model, and then fit the model, then made predictions.

I computed the accuracy score.

Objective 2: Train a SVM to detect breast cancer.

I took the scaled normalised training dataset used to train KNN algorithm

I trained the SVM Classifier on the training set, and %time the model

I fit the model and them used the fitted model to make predictions

I computed the accuracy for the models.

I described how I choose k=5

I printed the classification_report

I computed the accuracy score.
