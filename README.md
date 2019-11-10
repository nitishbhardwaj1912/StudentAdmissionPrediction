
# Student Admission Prediction
This repository contains objects related to the prediction of student admission based on historical data of students.

## Information on Dataset
The dataset[1] contains several parameters which are considered important during the application in Graduation Programs. The parameters included are : 
 1. GRE Scores ( out of 340 ) 
 2. TOEFL Scores ( out of 120 ) 
 3. University Rating ( out of 5 ) 
 4. Statement of Purpose and Letter of Recommendation Strength ( out of 5 ) 
 5. Undergraduate GPA ( out of 10 )
 6. Research Experience ( either 0 or 1 ) 
 7. Chance of Admit ( ranging from 0 to 1 )

## Business Problem
Train a Machine Learning model based on historical student data to predict the chances of admission for a set of students.

## Research Analysis Steps:
1. **Exploratory Data Analysis:** Understanding the dataset
2. **Cleaning:** Most part of the data is already cleaned in this dataset. However, renaming, dropping null values or irrelevant features etc have been performed in this process.
3. **Feature Selection:** The features that have a direct high impact on the target have been recognized in this process.
4. **Model Creation and Training:** In this process, four models are trained on the selected features and their accuracy is computed.
5. **Model Validation:** To validate the model, the cross validation technique is used. The result of validation is given below:
		Logistic Regression: 76.500000 (0.065383)
		K Nearest Neighbour: 84.500000 (0.071414)
		Decision Tree: 81.500000 (0.066332)
		Random Forest: 85.000000 (0.048734)
6. **Model Testing with real data:** In this process, the model is given real data and its performance is validated. An example of this process is given below:
		Status of Student with the following scores CGPA = -1, GRE = -1, TOEFL = -1 will be reject
		Status of Student with the following scores CGPA = 0, GRE = 340, TOEFL = 0 will be reject
		Status of Student with the following scores CGPA = 9, GRE = 320, TOEFL = 120 will be admit
		Status of Student with the following scores CGPA = 7, GRE = 300, TOEFL = 120 will be reject

## References:
[1] "A Comparison of Regression Models for Prediction of Graduate Admissions - IEEE Conference Publication", Doi.org, 2019. [Online]. Available: https://doi.org/10.1109/ICCIDS.2019.8862140. [Accessed: 12- Dec- 2018].
