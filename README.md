# Non-Linear Classification using Boosted Decision Trees, Random Forests, and SVM

This project explores the use of non-linear classifiers for classification of the Adult dataset. The project uses three software libraries for non-linear classification types: Boosted Decision Trees, Random Forests, and Support Vector Machines (SVM) with Gaussian Kernel. All of these are available in scikit-learn, although external libraries such as XGBoost and LibSVM can also be used.

## Dataset

The Adult dataset is used for this project. The dataset consists of two files: the training data file a9a with 32,561 samples, each with 123 features, and a9a.t with 16,281 test samples. The data is in LibSVM format, where each line takes the form <label> <feature-id>:<feature-value> <feature-id>:<feature-value> .... The scikit-learn library includes utility functions for loading datasets in the LibSVM format.

## Algorithms

### Boosted Decision Trees

Boosted Decision Trees is an ensemble learning method that uses decision trees as weak learners. It works by iteratively training a sequence of decision trees, where each subsequent tree focuses on the misclassified examples from the previous tree. XGBoost is used for implementing the Boosted Decision Trees algorithm.

### Random Forests

Random Forests is another ensemble learning method that uses decision trees as weak learners. It works by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees. Scikit-learn is used for implementing the Random Forests algorithm.

### Support Vector Machines with Gaussian Kernel

Support Vector Machines with Gaussian Kernel is a non-linear classifier that works by finding a hyperplane that separates the examples into different classes in the feature space. It uses a Gaussian Kernel function to map the data into a higher-dimensional space where a hyperplane can be found. Scikit-learn is used for implementing the SVM algorithm.

### Training Methodology

For each algorithm, hyperparameters are set and tuned to obtain the best performance. The hyperparameters include the type of kernel and regularization parameter for SVM, tree method, max depth, number of weak classifiers for XGBoost, and the number of estimators, min impurity decrease, and min samples leaf for Random Forests. Hold-out validation or K-fold cross-validation is used to evaluate the performance of the algorithms. The test error rates are computed after settling on the hyperparameter settings and training the final classifiers.

## Files

There are three files in this project:

1. BoostedDecisionTrees.ipynb - This file contains the implementation of the Boosted Decision Trees algorithm using XGBoost.

2. RandomForests.ipynb - This file contains the implementation of the Random Forests algorithm using scikit-learn.

3. SVM.ipynb - This file contains the implementation of the SVM algorithm using scikit-learn.

## Results
The list of hyperparameters and brief descriptions of each hyperparameter that were tuned in training, their default values, and the final hyperparameter settings used to obtain the best results are included in the project report. The training error rates, hold-out or cross-validation error rates, and test error rates for the final classifiers are also reported. A table with a column for each hyperparameter and the accuracy of each configuration of parameters is also included in the report.

The project aims to achieve the best achievable accuracy for each classifier on the given dataset. The amount of effort put into tuning the parameters will be determined based on the discrepancy between the accuracy obtained and the best achievable accuracy on the a9a data for each algorithm.

## Conclusion

The project demonstrates the use of non-linear classification algorithms - Boosted Decision Trees, Random Forests, and Support Vector Machines with Gaussian Kernel - to classify the Adult dataset. We implemented these algorithms using scikit-learn and other external libraries. We used the a9a dataset, which is available in LibSVM format, and trained the classifiers using hold-out validation or K-fold cross-validation. We tuned various hyperparameters for each algorithm and reported the training error rates, hold-out or cross-validation error rates, and test error rates for the final classifiers. We also reported other settings we tried and the corresponding accuracy achieved. Our goal was to obtain the best achievable accuracy for each classifier on the given dataset. Overall, this project demonstrated the importance of hyperparameter tuning and the effectiveness of non-linear classifiers in solving classification problems.

## Academic Integrity Statement

Please note that all work included in this project is the original work of the author, and any external sources or references have been properly cited and credited. It is strictly prohibited to copy, reproduce, or use any part of this work without permission from the author.

If you choose to use any part of this work as a reference or resource, you are responsible for ensuring that you do not plagiarize or violate any academic integrity policies or guidelines. The author of this work cannot be held liable for any legal or academic consequences resulting from the misuse or misappropriation of this work.

In summary, any unauthorized copying or use of this work may result in serious consequences, including but not limited to academic penalties, legal action, and damage to personal and professional reputation. Therefore, please use this work only as a reference and always ensure that you properly cite and attribute any sources or references used.
