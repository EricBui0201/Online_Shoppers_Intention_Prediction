# Online_Shoppers_Intention_Prediction

**1. Introduction**

***Dataset***

The dataset is downloaded from the Kaggle website. It was originally collected and provided by:
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

The dataset consists of 10 numerical and 8 categorical attributes among which the 'Revenue' attribute is used as the class label and is the target feature in our prediction model. (see Jupyter Notebook file for more details)

***Objectives***

The objective is to build a model to predict if the customer will be the product or not (categorical target feature).


**2. Techniques**

Since we have a categorical target feature, we need to use the classification algorithms which is part of the supervised machine learning.
In this project, I decided to use different algorithms so that we can compare the result between them: logistic regression, GaussianNB, KNN, SVC, Random Forest, Decision Trees, Adaboost, XGB, Catboost.

In addition to this, since the dataset of the target feature is unbalanced (more "Not buy" value than "buy" value), we also need to use the sampling techniques (Random Undersampling and SMOTE) to deal with this unbalanced dataset.

Furthermore, since we have many categorical independant attributes with multiple values, we can reduce the number of independant features and make them more condensed. It would improve the performance of our models.


**3. Outcomes**

KPIs: in our case, we have two values of the target feature which are "True" (Buy) or "False" (Not buy). We will focus on two following scores:

* Precision score: In fact, we are focusing more on people who will not buy the product in order to analyse the factors that could impact on the decision of these customers so that the company can solve issues and make them buy products. Thus, the precision score is a good indicator as it shows if the model is good enough at not considering an actual "not buy" case as a "buy" case.

* Accuracy score: since the dataset is unbalanced, it is also important to have a good overall accuracy score.  

Outcommes:
* Random Forest is the most performant model compared to other models
* PCA alone did not really improve the performance of all models
* The combination of Random Undersampling technique (to deal with the unbalanced dataset) and PCA slightly improved the performance of the models
* The combination of SMOT resampling technique and PCA had the most significant impact on the models than the previous solutions:
    
    Accuracy score: higher than 3rd run for most of model - range [64.8% , 82%]
        
        Highest rate: Random Forest
    
    Recall score: much higher - range [63% , 91%]
        
        Highest rate: KNN
    
    Precision score: much higher - range [63% , 80.6%]
        
        Highest rate: Random Forest 

**Please refer to the presentation file and the Jupyter Notebook file for more detailed findings**
