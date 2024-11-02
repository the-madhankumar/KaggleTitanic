# Titanic Survival Prediction

## Overview

This project aims to predict the survival of passengers on the Titanic using various machine learning algorithms. The dataset consists of passenger information such as age, sex, ticket class, and other features. The main objective is to preprocess the data, train models, and evaluate their performance.

## Datasets

The project utilizes two datasets:
- **train.csv**: Contains information about passengers and their survival status.
- **test.csv**: Contains information about passengers without the survival status, used for prediction.

## Libraries Used

- `numpy`: For numerical operations.
- `pandas`: For data manipulation and analysis.
- `seaborn`: For data visualization.
- `matplotlib`: For creating static, animated, and interactive visualizations.
- `sklearn`: For machine learning models and metrics.
- `xgboost`: For advanced boosting algorithms.

## File Structure

```
.
├── train.csv
├── test.csv
└── KaggleTitanic.ipynb  # Main script for the project
```

## Installation

To run this project, you need to have Python installed. You can install the required libraries using pip:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn xgboost
```

## Usage

1. Clone the repository:

   ```bash
   git clone [<repository-url>](https://github.com/the-madhankumar/KaggleTitanic)
   cd KaggleTitanic
   ```

2. Open `model.ipynb` and run the script:

   ```bash
   run each of the cell 
   ```

3. The script will:
   - Load the datasets.
   - Preprocess the data (handle missing values, drop irrelevant features, and perform one-hot encoding).
   - Train three different models: Logistic Regression, XGBoost, and Random Forest.
   - Print the accuracy of each model.

## Model Performance

The following accuracies were achieved using the respective models:

- **Logistic Regression**: 79.89%
- **XGBoost**: 79.33%
- **Random Forest**: 82.12%

## Preprocessing Steps

The preprocessing function performs the following steps:

- Combines the training and test datasets for consistent processing.
- Fills missing values in columns such as Age, Cabin, Embarked, and Fare.
- Extracts features from the Cabin column (letter and number).
- One-hot encodes categorical features (Sex, Cabin letters, and Embarked).
- Creates new features based on existing data.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss improvements.

## Acknowledgments

- The Titanic dataset is available on Kaggle and is a common dataset used for beginner machine learning projects.
- Special thanks to the authors of the libraries used in this project.
