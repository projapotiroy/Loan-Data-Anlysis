# Loan Data Anlysis
The task is to decide a person be eligible for taking the loan or not based on some feature including his/her gender, married, dependents, education, self employed, applicant income, coapplicant income, loan amount, loan amount term, credit history, and property area.

## Dataset
Dataset contains 13 columns and 367 rows. The columns are gender, married, dependents, education, self employed, applicant income, coapplicant income, loan amount, loan amount term, credit history, property area and loan approved. The outcome is loan approved that contains 0 and 1 values. 1 means the person is eligible for the loan and 0 means not eligible. The dataset contains numerical and categorical variables, some null values.  The distribution of the features are not normal, some are positively skewed, some are negatively skwed. There are outliers too. There occurs positive and negative correlation between the variables.

The dataset is  preprocessed before creating a model. All the unnecessary variables are removed. Null values are handled carefully. All the categorical values are converted to numerical using label encoder. I used Synthetic Minority Oversampling Technique (SMOTE) to balance the imbalanced dataset. After resampling, there are a total of 682 data, Each class contains a total of 341 data. The standardrization i.e standard scale normalization is performed. Feature is selected carefully. The dataset is split into 80% training and 20% test set.


## Model
I used five machine learning algorithms to build the model. The algorithms are-
1. Logistic Regression
2. K Nearest Neighbor (KNN)
3. Decision Tree
4. Random Forest
5. Support Vector Machine (SVM)


## Evaluation
Each model has been evalauted in terms of accuracy and loss. Log loss function is used.\
The sequence of the performance of the model is random forest > decision tree > knn > svm > logistic regression.\
Random forest model achieved an accuracy of 93.43% and 2.269 loss.
