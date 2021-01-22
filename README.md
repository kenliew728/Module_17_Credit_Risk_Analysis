# **Credit Risk Analysis**

## ***Overview***
The purpose of this analysis is to utilize six different machine learning models to predict credit risk based on credit card dataset from LendingClub, a peer-to-peer lending services company. 

The six machine learning models consist of:
1. Naive Random Oversampling
2. Synthetic Model Oversampling Technique (SMOTE)
3. Undersampling using Cluster Centroids Model
4. SMOTE and Edited Nearest Neighbors (SMOTEENN)
5. Balanced Random Forest Classifiers
6. Easy Ensemble AdaBoost Classifier

## ***Results***

### **Naive Random OverSampling**

#### *Accuracy Score*
Using the Random Oversampling method, it yielded a accuracy score of 0.65, which means the model only predicted correctly 65% of the time.

#### *Precision Score*
From the classification report, the model performed badly in predicting high risk group that are actually high risk due to low precision score of 0.01. In contrast, it performed better in predicting low risk group that are actually low risk with a score of 1.0

#### *Recall Score*
This model yielded a recall score of 0.72, which was better is labeling actual high risk group as high risk but not good at labeling actual low risk group as low risk with a score of 0.57, which means almost 50% of the actual high risk group was labeled as low risk. 

##### *Figure 1.1: Accuracy Score of Naive Random OverSampling*

![RandomOverSampling-Accuracy Score](https://user-images.githubusercontent.com/70525492/105403322-38e7ee00-5bee-11eb-9498-72f02daea82d.png)

##### *Figure 1.1: Precision & Recall Score of Naive Random OverSampling*
![RandomOverSampling-PreRecScore](https://user-images.githubusercontent.com/70525492/105403327-3a191b00-5bee-11eb-9193-83baf18c89b8.png)

### **SMOTE OverSampling**

#### *Accuracy Score*
Using the SMOTE Oversampling method, it yielded a accuracy score of 0.66, which means the model only predicted correctly 66% of the time.

#### *Precision Score*
From the classification report, the model performed badly in predicting high risk group that are actually high risk due to low precision score of 0.01. In contrast, it performed better in predicting low risk group that are actually low risk with a score of 1.0, and it is similar to the Naive OverSampling method. 

#### *Recall Score*
This model yielded a recall score of 0.63 for high risk group, which was better in labeling actual high risk group as high risk, but not as good as Naive Random OverSampling method. In other hand, it has a better recall score of 0.68 in labeling actual low risk group as low risk, and performed better than the Naive OverSampling method.  

##### *Figure 1.3: Accuracy Score of SMOTE OverSampling*
![SMOTE-Accuracy Score](https://user-images.githubusercontent.com/70525492/105540809-69965900-5cbc-11eb-9631-ac54482ca183.png)

##### *Figure 1.4: Precision & Recall Score of SMOTE OverSampling*
![SMOTE-PreRecScore](https://user-images.githubusercontent.com/70525492/105540810-69965900-5cbc-11eb-8097-232bb109df24.png)

### **Cluster Centroids UnderSampling**

#### *Accuracy Score*
Using the Cluster Centroids Undersampling method, it yielded a accuracy score of 0.54, which means the model only predicted correctly 54% of the time.

#### *Precision Score*
Similar to both of the oversampling methods, Cluster Centroids reported a score of 0.01 and 1.00 in predicting high risk and low risk group respectively. 

#### *Recall Score*
This model yielded a recall score of 0.67 for high risk group, which placed this model in between Random and SMOTE method. However, it fared worse than both oversampling methods with a recall score of 0.42.  

##### *Figure 1.5: Accuracy Score of Cluster Centroids UnderSampling*
![UnderSampling-Accuracy Score](https://user-images.githubusercontent.com/70525492/105541502-7798a980-5cbd-11eb-9b50-a881034991fc.png)

##### *Figure 1.6: Precision & Recall Score of Cluster Centroids UnderSampling*
![UnderSampling-PreRecScore](https://user-images.githubusercontent.com/70525492/105541504-7798a980-5cbd-11eb-815a-6718672c7d77.png)

### **SMOTEENN (Over and Under) Sampling**

#### *Accuracy Score*
Using the SMOTEENN Over and Under sampling method, it yielded a accuracy score of 0.67, which means the model only predicted correctly 67% of the time.

#### *Precision Score*
The SMOTEENN model was consitent with Random, SMOTE and Cluster Centroid sampling with a precision score of 0.01 and 1.00 respectively in predicting high risk and low risk groups. 

#### *Recall Score*
This model yielded a recall score of 0.80 for high risk group, which placed this model the top compared with the previous over and under sampling methods but has a score of 0.54 in labeling actual low risk group as low risk.

##### *Figure 1.7: Accuracy Score of SMOTEENN Over & Under Sampling*
![SMOTEEN-Accuracy Score](https://user-images.githubusercontent.com/70525492/105542083-669c6800-5cbe-11eb-8856-8d736c5e093f.png)


##### *Figure 1.8: Precision & Recall Score of SMOTEENN Over & Under Sampling*
![SMOTEEN-PreRecScore](https://user-images.githubusercontent.com/70525492/105542081-669c6800-5cbe-11eb-9d39-1e1d0603f44d.png)

### **Balanced Random Forest Classifier**

#### *Accuracy Score*
The Balanced Random Forest Classifier yielded a accuracy score of 0.79, which means the model only predicted correctly 79% of the time.

#### *Precision Score*
The Balanced Random Forest Classifier fared a little better with the rest of the model as it has a precision score of 0.03 and 1.00 respectively in predicting high risk and low risk groups. 

#### *Recall Score*
This classifier yielded a recall score of 0.70 for high risk group and 0.87 for low risk group. 

##### *Figure 1.9: Accuracy Score of Balanced Random Forest Classifier*
![BRF-Accuracy Score](https://user-images.githubusercontent.com/70525492/105543358-520c9f80-5cbf-11eb-8bc3-b634783353d4.png)

##### *Figure 2.0: Precision & Accuracy Score of Balanced Random Forest Classifier*
![BRF-PreRecScore](https://user-images.githubusercontent.com/70525492/105543360-520c9f80-5cbf-11eb-84e8-58cdf10ee7da.png)


### **Easy Ensemble AdaBoost Classifier**

#### *Accuracy Score*
The Balanced Random Forest Classifier yielded a accuracy score of 0.93, which means the model only predicted correctly 93% of the time.

#### *Precision Score*
The AdaBoost Classifier performed slightly better compared with the rest of the machine learningb models as it has a precision score of 0.09 and 1.00 respectively in predicting high risk and low risk groups. 

#### *Recall Score*
This classifier performed the best in labeling actual high risk and low risk groups with a recall score of 0.92 and 0.94 respectively. 

##### *Figure 1.9: Accuracy Score of Easy Ensemble AdaBoost Classifier*
![ABC-Accuracy Score](https://user-images.githubusercontent.com/70525492/105544928-196dc580-5cc1-11eb-9b1c-b72e32ef1acb.png)

##### *Figure 2.0: Precision & Accuracy Score of Easy Ensemble AdaBoost Classifier*
![ABC-PreRecScore](https://user-images.githubusercontent.com/70525492/105544929-196dc580-5cc1-11eb-984c-f66adee5fcee.png)

## ***Summary***

The table below displays the summary of accuracy, precision, recall, and F1 score of all the 6 machine learning models used in this analysis. 

Best Results: Easy Ensemble AdaBoost
Worst Results: Cluster Centroids Undersampling

##### *Figure 2.1: Summary of six machine learning models result*
![Picture5](https://user-images.githubusercontent.com/70525492/105547476-2a6c0600-5cc4-11eb-9f36-e42b8d23070d.png)


##### *Table 2.2: Confusion matrix for Easy Ensemble AdaBoost*
| Group     | Predicted True | Predicted False |
| --------- | -------------- | --------------- |
| High Risk | 93             | 8               |
| Low Risk  | 983            | 16121           |



Based on all six machine learning models, the Easy Ensemble AdaBoost has the best overall results compared to the rest. It performed exceptionally well in labeling groups that are actually high or low risk with a high recall score of 0.92 and 0.94 respectively, along with an accuracy score of 0.93. The confusion matrix also showed that majority of the group will be predicted high risk even if the applicants were low risk. In credit fraud detection, this would be a preferred model to use as the cost of predicting an actual high risk group as low risk will be high for the credit lending agency. It is better to over disqualified applicants in low risk group than to over qualified applicants in high risk group. The perfect example would be the sub-prime mortgages where high risk group qualified for a large mortgage loan, causing the 2008 financial crisis. 





