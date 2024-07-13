# HW 4 - Cancer and Diabeties analisys

## ECGR 5105 - Summer 2024

#### Joshua Ayers

#### SID: 801083470

#### Professor: Vinit Katariya

#### Github: https://github.com/Jayers0/HW4_ECGR5105

The goal of this assginment is to use the Skitlearn and pytorch ML frameworks and to implement SVM and SVR classifiers and then to compair their performance to the pervious labs self implemented frameworks. 


#### Problem 1
##### The objective of problem 1: 
The objective of problem 1 is to implement an SVM classifier and find the max number of K parameters to achive the max percision, reacall and acuriccy.

A Support Vector Machine (SVM) classifier is a supervised machine learning algorithm used for classification tasks. The SVM classifier works by finding the hyperplane that best separates the data points of different classes in the feature space. This hyperplane, known as the decision boundary, maximizes the margin between the closest points of the classes, which are called support vectors.

###### Sub Problem 1 - Identify the optimum number of K, principal components that achieve the highest classification accuracy. 

Linear kernel:
The optimal K seems to be 15 
- percision: 1.0
- Accuracy: 0.99
- Precision: 0.97

Polynomial Kernal:
The optimal K value seems to be 2 or 5
- percision: 1.0
- Accuracy: 0.89
- Precision: 0.7


Radial Basis Function (RBF):
- percision: 1.0
- Accuracy: 0.98
- Precision: 0.95

###### Sub Problem 2 - Plot your classification accuracy, precision, and recall over a different number of Ks.
See the HW4.ipynb file for graphs

###### Sub Problem 3 - Explore different kernel tricks to capture non-linearities within your data. Plot the results and compare the accuracies for different kernels.

As the data above shows 3 types of kernels
 
 - Linear: The polynomial kernel represents the similarity of vectors (training samples) in a feature space over polynomials of the original variables, allowing the classifier to fit more complex, non-linear boundaries.

- Polynomial: The polynomial kernel represents the similarity of vectors (training samples) in a feature space over polynomials of the original variables, allowing the classifier to fit more complex, non-linear boundaries.

- RBF: The RBF kernel, also known as the Gaussian kernel, maps the input space into an infinite-dimensional space. It measures the similarity between two points based on their distance

Results: The best was the RBF, followed by the linear and then finally the polynomial.

###### Sub Problem 4 - Compare your results against the logistic regression that you have done in homework 3.

Problem 3 - logistic regression on the data yealds
- Accuracy: 0.9912
- Precision: 1.0000
- Recall: 0.9767
- F1 Score: 0.9882


#### Problem 2

##### The objective of problem 2: 
The objective of problem 1 is to implement an SVM classifier and find the max number of K parameters to achive the max percision, reacall and acuriccy.

Support Vector Regression (SVR) is a type of Support Vector Machine (SVM) used for regression tasks. SVR is designed to predict continuous values. It works by finding a function that approximates the relationship between input features and a continuous target variable, while keeping errors within a certain margin.

##### Sub Problem 1 - Plot your regression model for SVR similar to the sample code provided on Canvas.

See HW4.ipynb for plots.

##### Sub Problem 2 - Compare your results against linear regression with regularization loss that you already did in assignment1. 



##### Sub Problem 3 - Use the PCA feature extraction for your training. Perform N number of independent training (N=1, …, K). Identify the optimum number of K, principal components that achieve the highest regression accuracy. 



##### Sub Problem 4 - Explore different kernel tricks to capture non-linearities within your data. Plot the results and compare the accuracies for different kernels.

See HW4.ipynb for plots.