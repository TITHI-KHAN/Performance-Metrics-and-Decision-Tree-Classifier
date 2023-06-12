# Performance-Metrics-&-Decision-Tree-Classifier

In pattern recognition, the performance of a classifier can be evaluated using various metrics that measure its accuracy and
effectiveness in recognizing and classifying different patterns. Some common metrics-

1. Confusion matrix: A confusion matrix is a table that summarizes the number of correct and incorrect predictions made by a
classifier. It provides a breakdown of how many patterns were classified into each category or class, as well as how many
patterns were misclassified.

2. Accuracy: Accuracy is a measure of how well a classifier performs in terms of the percentage of correctly classified patterns. It is
calculated as the ratio of the number of correctly classified patterns to the total number of patterns.

3. Precision and Recall: Precision measures the proportion of correctly classified patterns among those that were predicted to
belong to a particular class. Recall measures the proportion of correctly classified patterns among those that actually belong to a
particular class.

4. F1-score: The F1-score is a measure of the balance between precision and recall. It is calculated as the harmonic mean of
precision and recall and provides a single score that summarizes the overall performance of a classifier.

5. ROC curve and AUC: The Receiver Operating Characteristic (ROC) curve is a graphical representation of the trade-off between
the true positive rate and false positive rate for different classification thresholds.

These metrics can be used to evaluate the performance of a classifier on a test dataset, which is a separate dataset that is not used
during training. By comparing the performance of different classifiers using these metrics, we can select the best classifier for a
particular pattern recognition task.

# Confusion-Matrix

▪ TP: Algo predicts Yes, and
the actual value is Yes!

▪ FP: Algo predicts Yes, but
the actual value is No!

▪ FN: Algo predicts No, and
the actual value is Yes!

▪ TN: Algo predicts No, and
the actual value is No!

![image](https://github.com/TITHI-KHAN/Performance-Matrix-and-Decision-Tree/assets/65033964/8e82e583-f14f-4997-aef4-e5a4de3e0359)

# Accuracy / Recognition Rate

Accuracy = (TP + TN ) / (TP + FP + TN + FN)

▪ Condition positive (P).
▪ The number of real positive cases in the data.

▪ Condition negative (N).
▪ The number of real negative cases in the data.

# Precision / Positive Predictive Value (PPV)

PPV = True Positive / (True Positive + False Positive)

Precision = tp / ( tp + fp )

# Sensitivity, Recall, Hit Rate, or True Positive Rate (TPR)

TPR = True Positive / (True Positive + False Negative)

# False Positive Rate (FPR) or 1-Specificity

FPR = False Positive / (False Positive + True Negative)

# Specificity, Selectivity or True Negative Rate (TNR)

Specificity = True Negative / (True Negative + False Positive)

# Threat Score (TS) or Critical Success Index (CSI)

TS/CSI = True Positive / (True Positive + False Negative + False Positive )

# False Discovery Rate (FDR)

False Discovery Rate = False Positive / (True Positive + False Positive )

# Harmonic Mean, F-Measure

F-measure: harmonic mean of recall and precision:
= ( 2 * Precision * Recall ) / (Precision + Recall)

The harmonic mean is a type of average that is calculated as the reciprocal of the arithmetic mean of the reciprocals of a set of numbers. It is commonly used to calculate the average of rates, proportions, or ratios.

For example, if you have a set of values representing the speeds of different cars, and you want to calculate the average speed, you can use the harmonic mean to account for the fact that higher speeds have a greater impact on the overall average.

# ROC & AUC Curve

Receiver Operating Characteristic (ROC): Since, TPR is equivalent to Sensitivity and FPR is equal to 1 − specificity, the ROC graph is sometimes called the sensitivity vs (1 − specificity) plot. 

![image](https://github.com/TITHI-KHAN/Performance-Matrix-and-Decision-Tree/assets/65033964/f6070f78-6a5a-4201-8f22-c9d3648f2848)

Receiver Operating Characteristic (ROC): Since, TPR is equivalent to Sensitivity and FPR is equal to 1 − specificity, the ROC graph is sometimes called the sensitivity vs (1 − specificity) plot.

![image](https://github.com/TITHI-KHAN/Performance-Matrix-and-Decision-Tree/assets/65033964/3e8bc5b6-7788-497c-81cf-e0e7dc58875f)

The Area Under the Curve (AUC) measures a classifier’s ability to differentiate between classes and is used as a summary of the ROC curve. The higher the AUC, the better the performance of the model at distinguishing between the positive and negative classes.

▪ In general, an AUC of 0.5 suggests no discrimination (like the ability to diagnose patients with and without the disease or condition based on the test)
▪ 0.7 to 0.8 is considered acceptable
▪ 0.8 to 0.9 is considered excellent, and
▪ more than 0.9 is considered outstanding.
