# Mobile-Price-Range-Prediction

# Abstract:
**To predict “If the mobile with given features will be Economical or Expensive” is the main motive of this research work. Real Dataset is collected from websitehttps://www.kaggle.com Different feature selection algorithms are used to identify and remove less important and redundant features and have minimum    computational complexity. Different classifiers are used to achieve as higher accuracy as possible. Results are compared in terms of highest accuracy achieved and minimum features selected. Conclusion is made on the base of best feature selection algorithm and best classifier for the given dataset. This work can be used in any type of marketing and business to find optimal product (with  minimum cost and maximum features). To predict the accuracy of the mobile price range.**

# Problem Statement: 
**In the competitive mobile phone market companies want to understand sales data of mobile phones and factors which drive the prices
The objective is to find out some relation between features of a mobile phone(eg- RAM, Internal Memory, etc) and its selling price. In this problem, we do not have to predict the actual price but a price range indicating how high the price is**

# Dataset Information
![image](https://user-images.githubusercontent.com/74303124/147845355-f2e15e78-4778-4954-9282-90aac4268411.png)

# Introduction:
**Price is the most effective attribute of marketing and business. The very first question of costumer is about the price of items. All the costumers are first worried and thinks “If he would be able to purchase something with given specifications or not”.
Machine learning provides us best techniques for artificial intelligence like classification, regression, supervised learning and unsupervised learning and many more
Mobile now a days is one of the most selling andpurchasing device. Every day new mobiles with new version and more features are launched. Hundreds and thousands of mobile are sold and purchased on daily basis. So here the mobile priceclass prediction is a case study for the given type
of problem i.e. finding optimal product. The samework can be done to estimate real price of all
products like cars, bikes, generators, motors, fooditems, medicine etc.Many features are very important to beconsidered to estimate price of mobile. Forexample Processor of the mobile. Battery timingis also very important in today’s busy schedule of human being. Size and thickness of the mobile arealso important decision factors. Internal memory,Camera pixels, and video quality must be underconsideration. Internet browsing is also one of themost important constraints in this technological era of 21st century. And so is the list of many features based upon those, mobile price is decided. So we will use many of above mentioned features to classify whether the mobile would be very low, Medium, and High  or very_High.** 

# Result:
print(classification_report(y_test, y_pred))
              precision    recall  f1-score   support

           0       0.93      0.90      0.91       100
           1       0.79      0.80      0.80       100
           2       0.74      0.76      0.75       100
           3       0.87      0.86      0.86       100

    accuracy                           0.83       400
   macro avg       0.83      0.83      0.83       400
weighted avg       0.83      0.83      0.83       400

# Have a look at the feature importances according to decision tree model
# Feature	Score
# 0	ram	0.624663
# 1	battery_power	0.162317
# 2	pixels	0.132806
# 3	talk_time	0.017181
# 4	mobile_wt	0.014543
# Using Random Forest
print(classification_report(y_test, y_pred))
              precision    recall  f1-score   support

           0       0.93      0.95      0.94       100
           1       0.88      0.86      0.87       100
           2       0.81      0.89      0.85       100
           3       0.96      0.86      0.91       100

    accuracy                           0.89       400
   macro avg       0.89      0.89      0.89       400
weighted avg       0.89      0.89      0.89       400

# Let's get the important features for random forest.
# Feature Score 
# 0	ram	0.521100
# 1	battery_power	0.079214
# 2	pixels	0.076853
# 3	screen_size	0.040427
# 4	mobile_wt	0.040082

# Conclusions:
**This work can be concluded with the comparableresults of both Feature selection algorithms and classifier. This combination has achieved maximum accuracy and selected minimum but most appropriate features. It is important to note that in Forward selection by adding irrelevant or redundant features to the data set decreases the efficiency of both classifiers. While in backward selection if we remove any important feature from the data set, its efficiency decreases. The main reason of low accuracy rate is low number
of instances in the data set. One more thing should also be considered while working that converting a regression problem into classification problem introduces more error.**

