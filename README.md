# ada-2020-project-milestone-p3-p3-lwy
## Milestone P3:

### 1.	Title: Comparing Random Forest with Logistic Regression to predict a client ‘s subscription of a term deposit

### 2.	Abstract
The previous paper compares the logistic regression and random forest in predicting the rare political events, civil war. Also, the authors analyze the variable importance for random forests such as to determine the causes of civil war onset. We propose to study the power of random forest in predicting rare events in another field. We will use a dataset recording direct marketing campaigns (bank term deposit) of a Portuguese banking institution. The subscriptions of the bank term deposit are based on phone calls, so this is a rare event. We plan to apply random forest and logistic regression method to predict if a client will subscribe a term deposit in the bank, and compare their predictive accuracies. Then, we will analyze the causal effects in the subscription of a term deposit from a bank. Finally, we could indicate which clients are more likely to subscribe for term deposits. 

### 3.	Research questions
1. What is the accuracy of random forests in predicting the rare event in a new filed?

2. Can random forests predict the subscriptions of the bank term deposit efficiently and generally?

3. To what extent does random forest outperform logistic regression method in predicting the rare events, subscription of the bank term deposit?

4. Is there a causal effect of a client subscribing a bank term deposit?

5. What is the most important factor affecting a client subscribe a term deposit? Which clients are more likely to subscribe a term deposit?

### 4.	Proposed datasets
-	bank-additional-full.csv from “Bank Marketing Data Set” UCI machine learning repository. There are 41188 observations each with 20 features such as a client’s age, sex and job. The observations are ordered by date (from May 2008 to November 2010). The dependent variable is ‘y’ indicating whether a client subscribe the bank term deposit. 
The dataset is highly imbalanced because few people subscribe the bank term deposit. The ratio of subscribed (‘Yes’) bank term deposit and not ('no') subscribed in the data is roughly 1:70. In addition, there are missing or unknown values such as ‘education’, ‘housing’ and ‘loan’ in the dataset because some people would not like to tell their private information to the banking representative. We will discard the rows containing missing values. 

### 5.	Methods
Data collection: (a) Collect the dataset from UCI Machine learning Repository (b) Discard the rows containing missing values in the dataset (c) Determining the categorical features and numerical features (d) Visualize the relationship between features and dependent variable y (e) Get the proper features

Building the logistic regression model: After getting the proper dataset and features, we will use these data to build three logistic regression models with no regularization, L1 norm and L2 norm regularization, respectively. Then we use ten-fold cross validation to plot the ROC curve, and calculate the AUC score and F1 score of each model. Finally, we will get the best model.

Building the random forest model: After selecting proper features, we will build a random forest model with different hyperparameters. We will test different hyperparameters, and use ten-fold cross validation to calculate the average accuracy with 95% confidence intervals. Then, we select the best hyperparameters. 

Compare logistic regression model and random forest model: We use ten-fold cross validation to plot the ROC curve, and calculate the AUC score and F1 score of the best logistic regression model and the best random forest model respectively. Then, we compare the results.

Data analysis: We will visualize the variable importance by mean decrease in Gini Score of random forest model. Second, we analyze the importance of the features. Third, we will draw the partial dependence plots. We will analyze how the percentage of total votes for subscribing the bank term deposit changes over the range of each predictor. Finally, we summarize the causes of subscribing bank term deposits. Also, we indicate which clients are more likely to subscribe the bank term deposit.

### 6.	Proposed timeline
Week 1: Collecting data from UCI machine learning repository, and then clean them. Also, we visualize the relationship between each feature and dependent variable. Then, we will try to select the proper features. We will implement logistic regression models with different hyperparameters, and select the best one. We will implement random forest models with different hyperparameters, and select the best one. 

Week 2: Comparing the predictive performances of the best logistic regression model and random forest model. We will visualize the variable importance by mean decrease in Gini Score of random forest model. Then, we will draw the partial dependence plots. Finally, we analyze the causal effects of subscribing the bank term deposits.

Week 3: Continuing with analysis, preparing the data story and short video.

### 7.	Organization within the team
-	Bohan will handle downloading the dataset from UCI machine learning repository in week 1. Bohan will clean and preprocess the dataset. The resulting code and datasets will be shared with the other members of the team. 

-	At the end of week 1 (or earlier if time allows it), Zengyu will implement the logistic regression algorithm with different hyperparameters on the dataset. Zengyu will use cross validation to test and select the best hyperparameters of logistic regression model. Qunyou will focus on building random forest model with different hyperparameters. Qunyou will use cross validation to test and select the best hyperparameters model. The testing results of each model will be recorded for further process.

-	In week 2, Bohan will apply ten-fold cross validation to the best logistic regression model and the best random forest model. Bohan will plot the ROC curve, and calculate the AUC score and F1 score of each model. The results are compared at the same time.

-	In week2, Zengyu and Qunyou will visualize the variable importance by mean decrease in Gini Score of random forest model. Also, Zengyu and Qunyou will draw the partial dependence plots. 

-	At the end of week 2, we will work together, and discuss the results.

-	In week 3, Bohan and Zengyu will focus on writing the data story and preparing all needed figures and examples.

-	In week 3, Qunyou will focus on preparing the short video with the main ideas, and will discuss the resulting figures and values with Bohan and Zengyu.


