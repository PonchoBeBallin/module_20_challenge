# Credit Risk Analysis Report Overview of the Analysis
## Purpose of the Analysis
The purpose of this analysis is to assess the creditworthiness of borrowers using historical lending data. The dataset is imbalanced, with a higher number of healthy loans compared to risky loans.

## Data Preparation
### Data Source
The dataset includes historical lending activity from a peer-to-peer lending services company.

### Data Splitting
The data was split into training and testing sets using the train_test_split function.

## Modeling
### Logistic Regression with Original Data
#### Training
A logistic regression model was trained on the original dataset.

#### Evaluation
- Confusion Matrix:
[[18663, 102],
[56, 563]]

- Classification Report:
precision    recall  f1-score   support
macro avg      0.92      0.95      0.94     19384
weighted avg   0.99      0.99      0.99     19384

## Results
The model performed exceptionally well with an overall accuracy of 99%. The precision and recall for class 0 (healthy loans) were both very high, indicating that the model is very good at identifying healthy loans. For class 1 (risky loans), the precision was 0.85 and recall was 0.91, showing that the model is also quite effective at identifying risky loans, though there is still some room for improvement.

## Conclusion
This analysis demonstrates the importance of addressing class imbalance in credit risk modeling. The high accuracy and balanced performance metrics indicate that the logistic regression model, especially when combined with resampling techniques, can be a powerful tool for credit risk assessment. Future work could explore other resampling techniques or more complex models to further improve performance.