# Building-Damage-Prediction

## Table of Contents
- [Main Objective](#main-objective)
- [Brief Description](#brief-description)
- [Data cleaning and Feature engineering](#data-cleaning-and-feature-engineering)
- [Classifier Models](#classifier-models)
- [Best Performing Model](#best-performing-model)
- [Key Findings and Insights](#key-findings-and-insights)
# Main Objective
The main objective of this analysis is to predict if the structure of a build is subject to damage. This has become necessary due to the impact of environmental and climatic changes on the structure of a building. Conventional methods of building damage estimation require a large amount of time and financial resources. For this reason, in recent years, machine learning algorithms that produce faster and more economical results have become the research topics of interest in damage estimation.
# Brief Description
The dataset consists of features that would help us identify and classify building structure that are prone to severe damage. The dataset consists of 550 records and 14 features with severe damage column as our target. Shown below is a brief information of the features and data types of the dataset.

![Damage building data types](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/e487ee7b-2215-4b6a-a5e5-84939d998371)

# Data cleaning and Feature engineering
Data wrangling, Exploratory data analysis and feature engineering were performed before training the data. The dataset contains no missing value. columns with high cardinality such as the building_id column was dropped as this column is not necessary for our machine learning. There was imbalance in the dataset as the proportion of severe damages far outweighed the proportion of non-severe damages as shown below.

![Damage grade distribution](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/a49456dc-1d46-45c6-8249-4d0708737b5f)

We checked for multicollinearity in the dataset by performing a heat map plot to show the correlations among the features. 

![Heat map plot](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/425feaab-759b-471a-b1b6-e820a8b460c3)

# Classifier Models
The dataset was trained using logistic regression and three other classifiers such as KNearest neighbor classifier, Decision tree classifer and Random Forest classifier. All models used the same training and test splits and the same cross-validation method. The models were tune using hyper parameters and the best parameters were used for the prediction. Summary of the outcome of the result of the models on both the training and test data is shown below.

![Model plot](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/d182622e-943b-42a1-a4eb-c9f617a21b58)

# Best Performing Model
Random forest seems to yield the best result when compared to other models in consideration. The model did better at predicting buildings with severe damages but did fairly at predicting building structure with non-severe damages. The confusion matrix of random model classifier is shown below.

![best perform cm](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/831e1f64-3dbf-4ced-8f9f-b97faed43430)

# Key Findings and Insights
KNearest Neighbor classifier did poorly on predicting building structure with severe and non-severe when compared with other models under consideration. Random Forest Classifier performs best. Random Forest Classifier had a training accuracy of 73.8% and test accuracy of 73.6%. All the models under consideration did fairly well at predicting building structure with non-severe damages. This is due to the imbalance of the dataset. 
