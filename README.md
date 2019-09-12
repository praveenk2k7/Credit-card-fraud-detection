# Credit-card-fraud-detection
This repo reads kaggle credit card dataset and classifies the transaction as normal or fraudulent

**Description**

The aim of this project is to build a simple machine learning classifier algorithm to classify whether the transaction is normal or fraudulent. In the dataset to preserve the identity, only 28 princial component of the feature is given along with time and transaction amount.

Various Exploratory Data Analysis were performed to understand the data. The observation are as follows: 

  - The dataset contains 284,407 transactions.
  -The mean of amount transaction is 88 and the maximum amount transacted is 25692. Therefore the data is skewed to its right.
  -99.83% of the transactions in this data set were not fraudulent while only 0.17% were fraudulent. The dataset is heavily imbalanced.
  -more features are negatively corelated to the class label and only 3 features are postively corelated.
  
**Training Classification Algorithm**

To get a better feeling of which algorithm would perform best on our data, five different algorithms are chosen and cross-validation technique is applied to find which algorithm performs better. ROC-AUC is chosen as the metric to decide the best classifier.  

AUC - ROC curve is a performance measurement for classification problem at various thresholds settings. ROC is a probability curve and AUC represents degree or measure of separability. It tells how much model is capable of distinguishing between classes. Higher the AUC, better the model is at predicting 0s as 0s and 1s as 1s

five algorithms are: 

  LogisticRegression
  KNeighborsClassifier
  DecisionTreeClassifier
  Support Vector Machine
  RandomForestClassifier
	
**Results**

![image](https://user-images.githubusercontent.com/44360746/64770330-8f1b3a80-d57f-11e9-84ae-a7b1dec78d5e.png)

As observed Random classifier performs better than other classifiers and also witht the less standard deviation in our experiments.

Further, on testing the random classifier with balanced and imbalanced data, the classifier performed well in the balanced data while returning nearly 50% of the fraud transaction as normal transactions.


	

  
  
