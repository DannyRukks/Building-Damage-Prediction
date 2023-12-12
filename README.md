# Building-Damage-Prediction
# Main Objective
The main objective of this analysis is to predict if the structure of a build is subject to damage. This has become necessary due to the impact of environmental and climatic changes on the structure of a building. Conventional methods of building damage estimation require a large amount of time and financial resources. For this reason, in recent years, machine learning algorithms that produce faster and more economical results have become the research topics of interest in damage estimation.
# Brief Description
The dataset consists of features that would help us identify and classify building structure that are prone to severe damage. The dataset consists of 550 records and 14 features with severe damage column as our target. Shown below is a brief information of the features and data types of the dataset.

![Damage building data types](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/e487ee7b-2215-4b6a-a5e5-84939d998371)

# Data cleaning & Feature engineering
Data wrangling, Exploratory data analysis and feature engineering were performed before training the data. The dataset contains no missing value. columns with high cardinality such as the building_id column was dropped as this column is not necessary for our machine learning. There was imbalance in the dataset as the proportion of severe damages far outweighed the proportion of non-severe damages as shown below.

![Damage grade distribution](https://github.com/DannyRukks/Building-Damage-Prediction/assets/97890440/a49456dc-1d46-45c6-8249-4d0708737b5f)
