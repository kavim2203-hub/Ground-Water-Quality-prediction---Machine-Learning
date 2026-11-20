# Groundwater Quality Prediction Using Machine Learning

## Project Overview

This project aims to predict groundwater quality using machine learning classification techniques based on physicochemical water parameters.

The system classifies groundwater samples into three categories: **Good, Moderate, and Poor**. Multiple machine learning algorithms are implemented and compared to identify an effective model for groundwater quality assessment.

The project also incorporates Explainable AI techniques and Machine Unlearning to improve model transparency and study its performance after data removal.

## Problem Statement

Groundwater contamination is a major concern for public health and environmental sustainability. Traditional water quality assessment methods can be time-consuming and difficult to scale.

This project explores a data-driven approach to classify groundwater quality using machine learning models, helping identify potential water quality issues through physicochemical parameters.

## Technologies Used

- **Programming Language:** Python
- **Machine Learning:** Random Forest, SVM, KNN, XGBoost
- **Ensemble Learning:** Voting Classifier
- **Probabilistic Model:** Hidden Markov Model (HMM)
- **Data Processing:** Pandas, NumPy, Scikit-learn
- **Data Balancing:** SMOTE
- **Explainable AI:** SHAP, LIME
- **Experiment Tracking:** Weights & Biases (W&B)
- **Visualization:** Matplotlib

## Project Methodology

### 1. Data Preprocessing
- Cleaned and prepared groundwater quality data.
- Removed irrelevant features such as station identifiers and year.
- Classified samples based on conductivity thresholds.
- Applied label encoding to target categories.
- Used SMOTE to address class imbalance.
- Applied StandardScaler for feature standardization.

### 2. Machine Learning Models

Implemented and compared the following algorithms:

- **Random Forest:** Ensemble of decision trees for robust classification.
- **Support Vector Machine (SVM):** Classification using an RBF kernel.
- **K-Nearest Neighbors (KNN):** Classification based on neighboring data points.
- **XGBoost:** Gradient boosting for structured data classification.
- **Voting Classifier:** Combined predictions from Random Forest, Gradient Boosting, and AdaBoost using soft voting.
- **Hidden Markov Model (HMM):** Explored hidden-state patterns in groundwater data.

### 3. Model Evaluation

Evaluated model performance using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC Curve and AUC

Weights & Biases (W&B) was used for experiment tracking, performance comparison, and hyperparameter tuning.

### 4. Explainable AI 

Applied SHAP and LIME to interpret model predictions and understand the contribution of important groundwater parameters.

Key features identified include:
- Conductivity
- pH
- Temperature

These explanations help improve the interpretability of machine learning predictions.

### 5. Machine Unlearning

Explored machine unlearning to study how models perform after selected training data is removed.

Compared model performance before and after the unlearning process to understand prediction retention and model robustness.

## Results and Model Comparison

### Initial Test Performance

| Model             | Test Accuracy |
|-------------------|---------------|
| Random Forest     | 100%          |
| XGBoost           | 100%          | 
| Voting Classifier | 100%          |
| SVM               | 94%           |
| KNN               | 94%           |
| HMM               | 20%           |

SVM and KNN were further tuned using W&B.

### Performance After Machine Unlearning

| Model             | Test Accuracy |
|-------------------|---------------|
| Random Forest     | 100%          |
| Voting Classifier | 97.4%         |
| SVM               | 90.4%         |
| KNN               | 86.0%         |
| HMM               | 21.3%         |

**Key Finding:** Random Forest demonstrated the strongest reported performance and retained its classification accuracy after the unlearning process.

*Note: These are the results reported in the project experiments.*

## Key Features

- Groundwater quality classification into Good, Moderate, and Poor.
- Comparison of multiple machine learning algorithms.
- Class imbalance handling using SMOTE.
- Hyperparameter tuning and experiment tracking using W&B.
- Model interpretation using SHAP and LIME.
- Performance evaluation before and after machine unlearning.

## Applications

- Groundwater quality assessment.
- Environmental monitoring.
- Water safety analysis.
- Identifying potential contamination risks.
- Supporting data-driven water resource management.

## Conclusion

This project demonstrates the application of machine learning techniques to groundwater quality prediction.

Through model comparison, Explainable AI, and machine unlearning, the project explores prediction performance, model interpretability, and robustness after data removal.

Random Forest emerged as the strongest-performing model in the reported experiments, highlighting the potential of machine learning for environmental data analysis.

## Project Presentation

Refer to the uploaded PowerPoint presentation for the detailed methodology, model comparisons, visualizations, and experimental results.
