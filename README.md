# Day-89-Evaluation

###  Overview

**Model Evaluation** is the process of measuring how well a trained machine learning model performs on unseen data.

It helps determine whether the model is **accurate, reliable, and ready for deployment**.

---

##  Why Evaluation is Important?

* Checks model performance
* Detects overfitting/underfitting
* Compares different models
* Ensures real-world reliability

---

##  Evaluation Metrics (Classification)

###  Accuracy

```text
Accuracy = (Correct Predictions) / (Total Predictions)
```

---

###  Precision

```text
Precision = TP / (TP + FP)
```

---

###  Recall

```text
Recall = TP / (TP + FN)
```

---

###  F1 Score

```text
F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
```

---

###  Confusion Matrix

|                 | Predicted Positive | Predicted Negative |
| --------------- | ------------------ | ------------------ |
| Actual Positive | TP                 | FN                 |
| Actual Negative | FP                 | TN                 |

---

##  Evaluation Metrics (Regression)

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

---

##  Example (Python)

```python
from sklearn.metrics import accuracy_score, confusion_matrix

y_true = [0, 1, 1, 0]
y_pred = [0, 1, 0, 0]

print("Accuracy:", accuracy_score(y_true, y_pred))
print("Confusion Matrix:\n", confusion_matrix(y_true, y_pred))
```

---

##  Best Practices

- Use appropriate metrics based on problem type
- Evaluate on unseen/test data
- Use cross-validation for better reliability

---

## Key Takeaways

- Evaluation measures model performance
- Different metrics for classification and regression
- Essential before deployment

---

