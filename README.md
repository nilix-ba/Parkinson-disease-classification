# Parkinson's Disease Classification

This project aims to classify Parkinson's disease based on voice-related features. The dataset contains 767 samples with 771 columns, where 770 columns are features, and one column is the label (0 for not sick and 1 for sick).

## Getting Started

### Prerequisites

Before running the code, ensure you have the following libraries installed:

- `numpy`
- `pandas`
- `scipy`
- `matplotlib`
- `sklearn`

### Running the Code

1. Clone the repository or download the dataset (`pd_speech_features.csv`) to the same directory as your code.
2. Execute the provided Python script (`Parkinson-disease-classification.py`) to perform the classification task.

## Data Preprocessing

- The dataset is loaded from the `pd_speech_features.csv` file.
- Data types of each column are checked.
- Missing values are identified and reported.

## Variance Inflation Factor (VIF)

VIF is calculated to measure the strength of the correlation between the independent variables (features). High VIF values indicate high multicollinearity.

## Data Splitting

The dataset is split into training and testing sets using a 70-30 split ratio.

## Normalization

StandardScaler is used to normalize the dataset to ensure consistent feature scales.

## Handling Outliers

Outliers are removed from the training data to improve model performance.

## Model Evaluation

The following machine learning models are trained and evaluated:

1. **Decision Tree**
2. **K-Nearest Neighbors (KNN)**
3. **Support Vector Machine (SVM)**
4. **Random Forest**

For each model, the following steps are performed:

- Cross-validation to estimate the model's performance.
- Training the model on the training data.
- Predicting labels on both the training and testing sets.
- Calculating accuracy scores and creating confusion matrices for evaluation.

## Principal Component Analysis (PCA)

PCA is applied to the feature set to reduce dimensionality and improve model performance.

## Model Comparison

A comparison of model performance is presented, including accuracy scores and classification reports.

## Conclusion

The K-Nearest Neighbors (KNN) model consistently shows the best results in classifying Parkinson's disease, both before and after applying Principal Component Analysis (PCA). The code and analysis provide insights into classifying Parkinson's disease based on voice-related features.
