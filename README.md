# About This Work

This dataset appears to be from two extractions of Kickstarter projects (https://www.kickstarter.com/) from 2016 and 2018. The 2018 dataset was chosen because the currencies are already converted.

Estevão Macedo used this for his final project in the course "Introduction to Data Science" (2023), part of the Master's Program in Complex Systems Modeling at the University of São Paulo.

Kickstarter is a crowdfunding platform where people can raise funds during a campaign period. The goal of this analysis is to **predict project success or failure at the time of campaign announcement, comparing the models: Logistic Regression, Decision Tree, and Random Forest.**

The data is publicly available at: https://www.kaggle.com/datasets/kemical/kickstarter-projects

Thanks to Mickaël Mouillé for providing this dataset under the CC BY-NC-SA 4.0 license.

# Model Evaluation Metrics

**Accuracy**

*   Logistic Regression Accuracy: 0.6771
*   Decision Tree Accuracy:       0.6745
*   Random Forest Accuracy:       0.6866

**Precision**

*   Logistic Regression Precision: 0.6705
*   Decision Tree Precision:       0.668
*   Random Forest Precision:       0.6807

**Recall**
*   Logistic Regression Recall:    0.6771
*   Decision Tree Recall:           0.6745
*   Random Forest Recall:           0.6866

**F1-score**
*   Logistic Regression F1-score: 0.6685
*   Decision Tree F1-score:       0.6671
*   Random Forest F1-score:       0.6787

**AUC-ROC**
*   Logistic Regression AUC-ROC: 0.7255
*   Decision Tree AUC-ROC:       0.7253
*   Random Forest AUC-ROC:       0.745

**Confusion Matrix - Logistic Regression:**
|                      | Predicted: Negative | Predicted: Positive |
|----------------------|---------------------|----------------------|
| **Actual: Negative** | 14,413  | 3,550 |
| **Actual: Positive** | 6,137 | 5,900  |


**Confusion Matrix - Decision Tree:**
|                      | Predicted: Negative | Predicted: Positive |
|----------------------|---------------------|----------------------|
| **Actual: Negative** | 14,235  | 3,728  |
| **Actual: Positive** | 6,036  | 6,001  |


**Confusion Matrix - Random Forest:**
|                      | Predicted: Negative | Predicted: Positive |
|----------------------|---------------------|----------------------|
| **Actual: Negative** | 14,511  | 3,452 |
| **Actual: Positive** | 5,949  | 6,088  |


![ROC Curve Comparison.png](https://github.com/macedoestevaof/kickstarter_modeling/blob/main/ROC%20Curve%20Comparison.png)

# Conclusions

Random Forest performs best, showing better generalization and class discrimination.

The model uses only static, pre-launch features and does not consider campaign dynamics.

Given this limitation, predictive performance is reasonable.

This approach is useful for early risk assessment and decision-making before the campaign starts.
