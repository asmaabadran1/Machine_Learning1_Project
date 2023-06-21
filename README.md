# Machine_Learning_Project
-Titanic Survival Prediction :
This project aims to predict the survival of passengers aboard the Titanic using machine learning models.

## Dataset

The dataset used for this project is the Titanic dataset, which is available on Kaggle. The dataset contains information about passengers aboard the Titanic, including their age, gender, ticket class, and whether or not they survived. The dataset contains 891 instances and 12 features. 

The following preprocessing steps were performed on the data:

- Missing values in the "Age" and "Embarked" columns were imputed using KNN imputation.
- The "Cabin" feature was dropped due to a high percentage of missing values.
- Categorical features ("Pclass", "Sex", and "Embarked") were one-hot encoded.
- Numerical features ("Age", "SibSp", "Parch", and "Fare") were scaled using robust scaling.

## Exploratory Data Analysis

During exploratory data analysis, we found that:

The majority of passengers were in third class.



## Data Preparation

The preprocessed dataset was split into training, validation, and test sets using stratified sampling to preserve the class distribution in each set. The training set contained 80% of the data, and the validation and test sets contained 20% each.

## Modeling

Several machine learning models were trained on the training set, including logistic regression, decision tree, random forest, and support vector machine (SVM). The models were evaluated using the area under the receiver operating characteristic (ROC-AUC) curve on the validation set. 

Based on the results, the SVM and random forest models performed the best. 

## Conclusion

The final model was evaluated on the test set, and achieved an ROC-AUC score of 0.84. This indicates that the model is able to distinguish between survivors and non-survivors with high accuracy. 
## Repository Structure

- `data/`: contains the Titanic dataset.
- ML1_project.ipynb:  the Jupyter notebook used for exploratory data analysis, preprocessing, modeling, and evaluation.
- `README.md`: this file.

## References

- Titanic: Machine Learning from Disaster. Kaggle. https://www.kaggle.com/c/titanic

