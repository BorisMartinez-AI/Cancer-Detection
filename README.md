![image](https://github.com/BorisMartinez-AI/Cancer-Detection/assets/110473221/98e1fe4a-605c-4eb4-81c0-6bcd54ad9379)

# Comparative Analysis of Classification Algorithms for Breast Cancer Detection
    
## Objective

The main purpose of this project is to construct a prediction model for breast cancer using several classification algorithms and then make a comparative analysis of performance and accuracy. Models were deployed using four classification algorithms:

* Logistic Regression
* Support Vector Machine (SVM)
* K-Nearest neighbors
* Decision trees

## Confusion Matrices for all algorithms

![Confusion Matrix Algorithms](https://github.com/BorisMartinez-AI/Cancer-Detection/assets/110473221/8263e4e6-9ea5-4974-ae5a-737cbe8fe9bf)

## Accuracy Results

The project uses a dataset publicly available from the UCI Machine Learning Repository

https://archive.ics.uci.edu/dataset/15/breast+cancer+wisconsin+original

Hyperparameter tuning was performed in all the algorithms (using GridSearchCV from SKlearn) to find the combination that rendered best performance. The following table summarizes the algorithms used, accuracy scores achieved and best combination of parameters obtained through the hyperparemeter tuning process.


|Classification Algorithm|F1 score|Best parameters|
|--- |--- |--- |
|Logistic Regression|97.5%| 'C': 0.1, 'penalty': 'l2', 'solver': 'lbfgs'|
|SVM (Support Vector Machine)|96%| 'C': 10.0, 'gamma': 0.001, 'kernel': 'rbf'|
|K-Nearest neighbors | 97%| criterion='entropy', max_depth=4|
|Decision trees|97%| 'algorithm': 'auto', 'n_neighbors': 5, 'p': 2|

<br>
It can be seen that the four algortihms produce high accuracy, particularly logistic regression, K-NN and Decision trees with scores above 97%






