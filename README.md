# Online_Shoppers_Intention_Prediction

**1. Introduction**

***Dataset***

The dataset is downloaded from the Kaggle website. It was originally prepared and provided by:
* C. Okan Sakar
Department of Computer Engineering, Faculty of
Engineering and Natural Sciences, Bahcesehir University,
34349 Besiktas, Istanbul, Turkey

and

* Yomi Kastro
Inveon Information Technologies Consultancy and Trade,
34335 Istanbul, Turkey


The dataset consists of feature vectors belonging to 12,330 sessions (rows).
The dataset was formed so that each session would belong to a different user in a 1-year period to avoid any tendency to a specific campaign, 
special day, user profile, or period.

The dataset consists of 10 numerical and 8 categorical attributes among which the 'Revenue' attribute is used as the class label and is the target feature in our prediction model.

***Objectives***

The objective is to build a model to predict if the customer will be the product or not (categorical target feature).


**2. Techniques**

Since we have a categorical target feature, we need to use the classification algorithms which is part of the supervised machine learning.
In this project, I decide to use different algorithms so that we can compare the result between them: logistic regression, GaussianNB, KNN, SVC, Random Forest, Decision Trees, Adaboost, XGB, Catboost.

In addition to this, since the dataset of the target feature is unbalanced, we also need to use the sampling techniques (Random Undersampling and SMOTE) to deal with this unbalanced dataset.

Furthermore, since we have many categorical independant attributes with multiple values, we can reduce the number of independant features and make them more condensed. It would improve the performance of our models.


**3. Outcomes**
