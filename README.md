# Titanic-Survival-Prediction

## Problem Statement

Predict whether a passenger survived the Titanic disaster using machine learning techniques.

## Dataset

* Source: Kaggle Titanic Dataset
* Training samples: 891
* Test samples: 418

## Feature Engineering

Created:

* Title (extracted from Name)
* FamilySize
* One-hot encoding for Embarked

Final features:

```python
[
    'Pclass',
    'Sex',
    'Age',
    'Fare',
    'Embarked_Q',
    'Embarked_S',
    'FamilySize',
    'Title'
]
```

## Model

```python
RandomForestClassifier(
    n_estimators=300,
    max_depth=5,
    min_samples_split=10,
    min_samples_leaf=5,
    random_state=42
)
```

## Evaluation

| Metric                    |   Score |
| ------------------------- | ------: |
| Validation Accuracy       |  81.56% |
| Cross Validation Accuracy |  82.71% |
| Kaggle Public Score       | 0.78708 |

## Feature Importance

Feature importance analysis was performed to understand the relative contribution of each feature to model predictions.

## Key Learnings

* Data cleaning
* Feature engineering
* One-hot encoding
* Label encoding
* Random Forest classification
* Hyperparameter tuning
* Cross-validation
* Feature importance analysis
* Overfitting vs. generalisation

## Future Improvements

* Try XGBoost
* Experiment with ensemble methods
* Perform more advanced feature engineering
