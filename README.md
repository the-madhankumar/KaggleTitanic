# Titanic Survival Prediction

## Overview

This project aims to predict the survival of passengers on the Titanic using various machine learning algorithms. The dataset consists of passenger information, such as age, sex, ticket class, and other features. The main objectives are to preprocess the data, train multiple models, and evaluate their performance, ultimately providing insights into the factors influencing survival rates.

## Datasets

The project utilizes two datasets:
- **train.csv**: Contains information about passengers along with their survival status.
- **test.csv**: Contains information about passengers without the survival status, which is used for prediction.

## Libraries Used

This project leverages several key Python libraries:
- `numpy`: For efficient numerical operations.
- `pandas`: For data manipulation and analysis.
- `seaborn`: For data visualization and statistical graphics.
- `matplotlib`: For creating static, animated, and interactive visualizations.
- `scikit-learn`: For implementing machine learning models and evaluation metrics.
- `xgboost`: For gradient boosting algorithms.
- `dvc`: For data version control, enabling reproducibility and collaboration.

## File Structure

```
├── train.csv 
├── test.csv 
├── gender_submission.csv
├── model.ipynb # Main script for the project
└── submission.csv
```

## Installation

To run this project, ensure you have Python installed along with DVC. Install the required libraries using pip:

```bash
pip install -r requirements.txt
```

To install DVC, use:

```bash
pip install dvc
```

## Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/the-madhankumar/KaggleTitanic
   cd KaggleTitanic
   ```

2. **Initialize DVC and pull the data:**

   ```bash
   dvc init
   dvc pull
   ```

3. **Open the notebook and run the script:**

   ```bash
   jupyter notebook notebooks/KaggleTitanic.ipynb
   ```

4. The script will:
   - Load the datasets.
   - Preprocess the data (handle missing values, drop irrelevant features, and perform one-hot encoding).
   - Train three different models: Logistic Regression, XGBoost, and Random Forest.
   - Print the accuracy of each model and save the trained models and metrics.

## Model Performance

The following accuracies were achieved using the respective models:

- **Logistic Regression**: 79.89%
- **XGBoost**: 79.33%
- **Random Forest**: 82.12%

## Preprocessing Steps

The preprocessing function implements the following steps:

- Combines the training and test datasets for consistent processing.
- Fills missing values in critical columns such as Age, Cabin, Embarked, and Fare.
- Extracts features from the Cabin column (both letter and number).
- Applies one-hot encoding to categorical features (Sex, Cabin letters, and Embarked).
- Creates new features based on existing data to enhance model training.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to discuss improvements or enhancements.

## Acknowledgments

- The Titanic dataset is available on [Kaggle](https://www.kaggle.com/c/titanic) and serves as a foundational dataset for machine learning projects.
- Special thanks to the authors and maintainers of the libraries used in this project for their contributions to the data science community.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Key Enhancements:
1. **DVC Section**: Added a dedicated section to highlight DVC's role in the project, including data management practices.
2. **File Structure**: Enhanced the file structure to include data directories, model files, and requirements.
3. **Installation Instructions**: Clear instructions for setting up DVC alongside the project dependencies.
4. **Notebooks Directory**: Organized the Jupyter notebook under a dedicated directory for clarity.

Feel free to customize any sections or details as needed!
