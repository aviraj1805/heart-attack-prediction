# Heart Attack Prediction - Regression Model Evaluation

A comprehensive machine learning project comparing Logistic Regression, LASSO Regression, and Ridge Regression for heart attack risk prediction.

## Project Overview

This project implements and evaluates three regularized regression techniques to predict the likelihood of a patient experiencing a heart attack based on clinical health metrics. The analysis focuses on model performance comparison and the impact of feature regularization on prediction accuracy.

Key Techniques:
- Logistic Regression - Standard classification baseline
- LASSO Regression - L1 regularization for feature selection
- Ridge Regression - L2 regularization for handling multicollinearity

## Dataset

Source: UCI Heart Disease Dataset / Kaggle Heart Attack Analysis Dataset
- Samples: Multiple patient records with clinical measurements
- Features: 13 clinical and demographic variables (pre-processed)
- Target Variable: Binary classification (0: No disease, 1: Heart disease present)

Key Features Include:
- Age, Sex
- Chest Pain Type (cp)
- Resting Blood Pressure (trestbps)
- Serum Cholesterol (chol)
- Fasting Blood Sugar (fbs)
- Resting Electrocardiographic Results (restecg)
- Maximum Heart Rate Achieved (thalach)
- Exercise-Induced Angina (exang)
- ST Depression (oldpeak)
- Slope of ST Segment (slope)
- Number of Major Vessels (ca)
- Thalassemia (thal)

## Technologies and Libraries

- Python 3.x
- Pandas - Data manipulation and analysis
- NumPy - Numerical computing
- Scikit-Learn - Machine learning algorithms
- Matplotlib & Seaborn - Data visualization

## Project Structure

```
heart-attack-prediction/
├── README.md                          # Project documentation
├── heart.csv                          # Raw dataset
├── heart_Normalization.ipynb          # Data preprocessing and normalization
├── heat.ipynb                         # Model implementation and evaluation
└── requirements.txt                   # Project dependencies
```

## Getting Started

### Prerequisites

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### Installation

```bash
git clone https://github.com/aviraj1805/heart-attack-prediction.git
cd heart-attack-prediction
```

### Running the Project

1. Data Preprocessing:
   - Open heart_Normalization.ipynb in Jupyter Notebook
   - Execute cells to normalize and prepare the dataset
   - Output: Cleaned and normalized dataset ready for modeling

2. Model Training and Evaluation:
   - Open heat.ipynb in Jupyter Notebook
   - Execute cells to train all three models
   - Review performance metrics and comparisons

## Methodology

### Data Preprocessing

- Handling missing values
- Feature normalization and standardization
- Train-test split (80/20 ratio)
- Feature scaling for regression models

### Model Implementation

Logistic Regression
- Standard classification model
- Serves as baseline for comparison
- No feature regularization

LASSO Regression (L1)
- Applies L1 penalty to coefficients
- Performs automatic feature selection
- Forces some coefficients to zero
- Useful when multicollinearity is present

Ridge Regression (L2)
- Applies L2 penalty to coefficients
- Shrinks less important features
- Retains all features in the model
- Handles multicollinearity effectively

### Evaluation Metrics

- Accuracy
- Precision and Recall
- F1-Score
- ROC-AUC Score
- Cross-validation scores
- Mean Squared Error (MSE)

## Key Findings

The project evaluates which regularization approach provides:
- Better prediction accuracy
- Improved generalization to unseen data
- Optimal feature importance handling
- Robustness against overfitting

## Results Summary

Comparative analysis of model performance will show:
- Baseline Logistic Regression performance
- LASSO's effectiveness in feature reduction
- Ridge's advantage in handling correlated features
- Optimal hyperparameter values for each model

## Insights and Applications

Clinical Applications:
- Early identification of high-risk patients
- Supporting preventive healthcare interventions
- Resource allocation in medical facilities

Technical Insights:
- Impact of regularization on model complexity
- Trade-offs between bias and variance
- Feature importance in heart disease prediction

## Hyperparameter Tuning

Models are evaluated with various regularization strengths:
- LASSO: Alpha parameter optimization
- Ridge: Lambda parameter optimization
- Cross-validation: K-fold validation for robust evaluation

## Project Notes

- Data normalization is critical for regression models
- Feature scaling ensures fair coefficient comparison
- Regularization strength should be tuned for optimal performance
- Class imbalance (if present) should be addressed appropriately

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (git checkout -b feature/improvement)
3. Commit changes (git commit -am 'Add improvement')
4. Push to branch (git push origin feature/improvement)
5. Open a Pull Request

## References

- UCI Heart Disease Dataset: https://archive.ics.uci.edu/ml/datasets/heart+disease
- Kaggle Heart Attack Dataset: https://www.kaggle.com/rashikrahmanpritom/heart-attack-analysis-prediction-dataset
- Scikit-Learn Documentation: https://scikit-learn.org/

## License

This project is open source and available under the MIT License.

## Author

Aviraj - Machine Learning Enthusiast

For questions or suggestions, feel free to open an issue or contact through GitHub.

---

Last Updated: 2024
Status: Active Development
