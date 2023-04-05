# Traffic-data-analysis

Traffic data analysis is a very important process to solve the problem of urban traffic congestion. Through traffic data analysis, you can determine the causes of traffic jams and find ways to solve them.

### Traffic Data Collection
Traffic data can be collected in a number of ways. Typical methods include traffic cameras, vehicle recognition sensors, and GPS. By collecting this data, you can get information about where traffic jams occur, traffic volume, vehicle speed, and more.

### How to analyze traffic data
Traffic data analysis requires various analysis methods. Representative methods include cluster analysis, regression analysis, and time series analysis. These analytical methods can be used to determine the causes of traffic jams and find ways to solve them.

### Application of traffic data analysis
Traffic data analysis can be applied in various fields. For example, it can be used to widen roads to solve traffic congestion or improve public transportation. In addition, it can be applied to marketing strategies such as advertising campaigns or events by identifying traffic jam times through traffic data analysis.

## Traffic data analysis (binary classification)

### Analysis purpose

- Development of a machine learning-based accident classification model for traffic accident data
- Identification of factors affecting the occurrence of traffic accidents through analysis results
- Interpretation using explainable artificial intelligence (XAI) techniques for analysis results of classification models

### Introduction to data

- Response variable: whether an accident occurred (0: no occurrence, 1: an accident occurred)
- Explanatory variables: A total of 37 variables consisting of the characteristics of the driving road (width of the road, whether there are speed bumps, whether there are traffic lights, whether there are center barriers, …) and the traffic volume of the road

### Analysis process

1. Pretreatment
    
     1-1. Check the characteristics of variables and the presence or absence of missing values
    
     1-2. Data correction using oversampling, undersampling, and hybrid sampling techniques to solve the imbalance problem of response variables
    
     1-3. Variable preprocessing through One-Hot Encoding for categorical variables and standardization and normalization through StandardScaler for continuous variables
    
     1-4. Divided into training data and test data in a ratio of 7:3
    
2. Modeling
    
     2-1. Model learning progress through training data for a total of 6 machine learning models (RandomForest, CatBoost, SVM, NaiveBayes, XGBoost, LightGBM)
    
     2-2. Confirmation of optimal classification performance for each model through hyperparameter optimization
    
     2-3. Identify the machine learning model that performs optimally for four performance evaluation measures (accuracy, precision, recall, F1-score)
    
3. Explainable artificial intelligence (XAI; eXplainable AI)
    
     3-1. Identification of factors affecting traffic accidents using SHAP, an XAI technique, for classification results of machine learning models with optimal performance
    
     3-2. Analysis of the classification result of the model using Partial Dependence Plot (PDP) and Shapley Additive exPlanations (SHAP) for the classification result of the model


## Traffic data analysis (multi-class classification)

### Analysis purpose

- Development of a machine learning-based injury classification model for traffic accident data
- Identification of factors affecting the degree of driver's injury in the event of an accident through analysis results
- Interpretation using explainable artificial intelligence (XAI) techniques for analysis results of classification models

### Introduction to data

- Response Variable: Driver's Injury Degree (0: Minor Injury, 1: Serious Injury, 2: Fatal Injury)
- Explanatory variables: A total of 49 variables consisting of driver characteristics (gender, age, drinking status, …) and road information (highway, national highway, …)

### Analysis process

1. Pretreatment
    
     1-1. Check the characteristics of variables and the presence or absence of missing values
    
     1-2. Determine the ratio of the three response variables
    
     1-3. Variable pre-processing through One-Hot Encoding for categorical variables
    
     1-4. Divided into training data and test data in a ratio of 7:3
    
2. Modeling
    
     2-1. Model learning progress through training data for a total of 7 machine learning models (Logistic Regression, RandomForest, CatBoost, SVM, NaiveBayes, XGBoost, LightGBM)
    
     2-2. Confirmation of optimal classification performance for each model through hyperparameter optimization
    
     2-3. Identify the machine learning model that performs optimally for four performance evaluation measures (accuracy, precision, recall, F1-score)
    
3. Explainable artificial intelligence (XAI; eXplainable AI)
    
     3-1. Identification of factors affecting the degree of driver injury by comparing the variable importance in machine learning and variable importance in SHAP for the classification results of the machine learning model with optimal performance
    
     3-2. Interpretation of the classification result of the model using LIME for the classification result of the model





```bash
├── hyperparameter_tuning.ipynb
├── traffic_data_binary_classification.ipynb
├── traffic_data_multiclass_classification.ipynb
└── traffic_data_xai.ipynb
```
