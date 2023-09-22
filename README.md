# Stroke Prediction
## Analyzing Patient Medical and Lifestyle Data to Predict Likelihood of a Stroke

**Author**: Fiyona Kriel

### Business problem:

The purpose of this analysis is to use various individual and lifestyle data to predict whether a patient is likely to have a stroke. Accurate stroke prediction can not only save lives, but also assist stakeholders to recognise contributing factors in order to develop effective treatment plans and preventative measures.

### Stakeholders:
- Medical Team: Doctors, Surgeons (neurologists) and other support staff to assist with effective diagnosis, treatment and prevention plans
- Medical Aid companies: to identify at-risk clients and tailor benefits and plans more effectively

### Data:
Data Source: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

Description of Data:
- According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths.
  This dataset is used to predict whether a patient is likely to get a stroke based on the input parameters like gender, age, various diseases, and smoking status.
- The target feature is stroke: 1 if the patient had a stroke or 0 if not
- For this dataset, there were 5110 rows and 12 columns.
- Each row in the data provides relevant information about the patient.

### Analytical Insights

#### Insight 1 - Glucose Level vs Heart Disease

![image](https://github.com/FiyonaK/Project-2/assets/138833676/e8a75ffe-2c22-43f4-b697-5d67e37a26d3)

In this visual we explored the relationship between a person's average glucose level and heart disease in predicting a stroke. Interestingly enough, in both cases, a higher average glucose level seems to contribute to a stroke, regardless of whether the individual presents with heart disease or not.

Additionally, it should be noted that higher average glucose levels may also contribute to the development of heart disease in an individual.

#### Insight 2 - Hypertension vs Smoking

![image](https://github.com/FiyonaK/Project-2/assets/138833676/7827bdb9-ccca-4b67-8801-430f7f1f85f3)

In the above visual we explored the relationship between smoking and hypertension. As can be seen from the above, the highest number of hypertensive cases presented in those who have never smoked! There are lower cases of hypertension in those that currently smoke, and those who have stopped smoking.

This is the complete opposite to what was expected. It seems that, according to our data, smoking does not play a big part in causing hypertension, if at all.

### Machine Learning Models

The following models were used:

    Linear Regression Model
    K Nearest Neighbours Classification Model (KNN)  
    Random Forest Classification ModeL

### Model Metrics

The best performing model was the KNN Model with PCA applied with the following metrics on the test data:

Accuracy: 93%

Precision: 33%

Recall: 1%

ROC AUC: 62%

### Summary and Recommendations

There are various lifestyle factors within an individual's control that could contribute to the likelihood of a stroke. In this particular scenario our aim is to have fewer false negatives, as these could be detrimental to a patient's diagnosis, and possibly life-threatening.

Recommendations:
- This was a highly imbalanced dataset, which could be contributing to the low precision and recall scores we are seeing. I recommend meeting with stakeholders to identify ways to balance the dataset a bit more, so our model is able to make more accurate predictions, specifically where reducing false negatives are concerned.
- These predictions will highlight patterns in health and lifestyle factors that could allow stakeholders to create effective prevention and treatment plans in order to reduce the overall number of stroke related incidents and/or deaths.

### For further information

For any additional questions, please contact:
  - Fiyona Kriel
  - fkriel@oldmutual.com 
