Title: Predicting Credit Card Fraud Using Machine Learning Models: A Comparative Study

Abstract:
Credit card fraud detection is a critical issue in financial security. In this study, we compare the performance of two machine learning models, logistic regression and random forest, in detecting fraudulent transactions. Using a publicly available dataset, we evaluate the models based on precision, recall, and F1-score. Our findings indicate that the random forest model outperforms logistic regression in identifying fraudulent transactions, providing a higher recall and F1-score.

Keywords: Machine Learning, Credit Card Fraud, Logistic Regression, Random Forest, Fraud Detection

1. Introduction

The rapid increase in online transactions has led to a corresponding rise in credit card fraud, posing significant financial risks. Detecting fraudulent transactions is a challenging problem due to the highly imbalanced nature of the data, where fraudulent transactions are much rarer than legitimate ones. This paper explores the effectiveness of logistic regression and random forest models in detecting credit card fraud. Our aim is to determine which model offers better performance in identifying fraudulent activities.

2. Related Work

Previous research has employed various machine learning algorithms to tackle credit card fraud detection. Logistic regression is often used for its simplicity and interpretability (Wang et al., 2018). More complex models like random forests have also been widely adopted due to their ability to handle non-linear relationships and interactions between features (Zhang & Li, 2019). This study builds on these approaches by directly comparing the two models using the same dataset.

3. Methodology

3.1. Dataset
We use a publicly available credit card fraud dataset, which contains transactions made by European cardholders in September 2013. The dataset includes features such as transaction amount, time, and anonymized features derived from the original features to protect user privacy. The dataset is highly imbalanced, with fraudulent transactions accounting for only 0.17% of all transactions.

3.2. Models

Logistic Regression: A linear model that predicts the probability of a transaction being fraudulent based on the input features.
Random Forest: An ensemble model that builds multiple decision trees and merges them to get a more accurate and stable prediction.
3.3. Evaluation Metrics
Given the imbalanced nature of the dataset, we focus on:

Precision: The ratio of correctly predicted fraudulent transactions to the total predicted fraudulent transactions.
Recall: The ratio of correctly predicted fraudulent transactions to the total actual fraudulent transactions.
F1-Score: The harmonic mean of precision and recall, providing a single metric that balances both.
4. Experiments and Results

4.1. Model Training
The dataset was split into 80% training and 20% testing sets. Both models were trained using the training data, with hyperparameters tuned via cross-validation.

4.2. Results

Model	Precision	Recall	F1-Score
Logistic Regression	0.84	0.62	0.71
Random Forest	0.91	0.76	0.83
The random forest model outperformed logistic regression, especially in terms of recall and F1-score, indicating its superior ability to identify fraudulent transactions.

5. Discussion

The results show that the random forest model provides a significant improvement in detecting fraudulent transactions over logistic regression. This can be attributed to the model's ability to capture complex patterns and interactions among features, which is particularly important in fraud detection where the data is often non-linear and highly imbalanced. However, the trade-off is that random forests require more computational resources and are less interpretable than logistic regression.

6. Conclusion

In this study, we compared logistic regression and random forest models for credit card fraud detection. The random forest model demonstrated better performance, especially in recall and F1-score, making it a more suitable choice for identifying fraudulent transactions in highly imbalanced datasets. Future work could explore the use of more advanced techniques such as deep learning or hybrid models to further improve detection accuracy.
