# Supervised-ML-Classification
Bank Marketing Effectiveness Prediction

Intoduction

Banks generally do an advertising cmpaign to get more funds from customers or give more loans.
In this project a bank of Portugal is trying to enroll customers in a Term Deposit by runnaing a marketing Campaign.
This project discusses the prediction model of Bank Marketing Effectiveness of a Portuguese Marketing institution. The marketing campaigns were based on phone calls. 

🎯 The classification goal is to predict if the client will subscribe to a term deposit.

Attribute Information

Input variables:

Bank Client data:
age (numeric)

job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')

marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)

education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')

default: has credit in default? (categorical: 'no','yes','unknown')

housing: has a housing loan? (categorical: 'no','yes','unknown')

loan: has a personal loan? (categorical: 'no','yes','unknown')

Related with the last contact of the current campaign:

contact: contact communication type (categorical: 'cellular','telephone')

month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')

day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')

duration: last contact duration, in seconds (numeric).

Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

Other attributes:

campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)

pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)

previous: number of contacts performed before this campaign and for this client (numeric)

poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')

Output variable (desired target):

y - has the client subscribed a term deposit? (binary: 'yes','no')


Steps

First I explore the data, cleaned and preprocessed the data and then I performed the exploratory data analysis to extract information, in which we identified certain trends, relationships, correlation and found out the features that had some impact on our dependent variable and plotted the graph to visualize the impact on dependent variable. I also encoded the categorical variables. 

I build the various machine learning algorithms on our split and standardized data. I tried different algorithms namely; Logistic Regression, Random Forest Classifier, Decision Tree Classifier, Gradient Boosting Classifier, K Neighbors Classifier, XG Boost and Naive Bayes Classifier. I did hyper parameter tuning and evaluated the performance of the model. 

Conclusion

We can choose our model either Gradient Boosting Classifier, Random Forest Classifier and XG boost to predict Effectiveness as they are showing maximum accuracy with 0.88,0.89 and 0.88 resp.
