# PIMA Diabetes Classification Project

This project leverages Python to perform exploratory data analysis (EDA), feature selection, and classification on the **PIMA Diabetes dataset**, which contains diagnostic data for predicting diabetes in women. The dataset consists of 750 samples and 8 diagnostic features, such as glucose levels, blood pressure, and BMI, along with the target outcome (positive/negative diabetes test).

## Key Features

### Exploratory Data Analysis (EDA)
- Evaluated data distributions, detected outliers, and examined correlations between features and the target variable.
- Histograms revealed that some features (e.g., insulin, BMI) were highly skewed, while others (e.g., glucose, blood pressure) were normally distributed.
- Boxplots identified outliers, particularly in insulin and skin thickness measures.

#### Data Preprocessing
- Replaced medically impossible zero values in glucose, blood pressure, skin thickness, insulin, and BMI using mean or median values based on distributions.
- Standardized features for consistent scaling.

#### Feature Selection
- Pearson correlation analysis guided feature selection by identifying significant predictors of diabetes (e.g., glucose, BMI, age).

![download](https://github.com/user-attachments/assets/62f83bd1-95d3-40de-af04-2284513bb34c)
![download (1)](https://github.com/user-attachments/assets/bf6e4f2e-eae3-4a11-917e-ea21c89d2697)

### Model Training
- Multiple logistic regression models were trained on various feature subsets.
- Achieved the best accuracy using all features and a second-best result with only four highly correlated features.

### Outcome Prediction
- Predicted diabetes outcomes for new samples using the best-performing model, with probabilities calculated for each prediction.



## Tools and Libraries
- **Python Packages**: NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn
- **Machine Learning**: Logistic Regression

## Key Results
- The final model successfully predicted outcomes for new data samples, achieving robust accuracy with logistic regression.
- The inclusion of preprocessing steps like handling missing values and feature selection improved model performance.

## How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Python-PIMA-classification.git
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Python scripts for EDA, model training, and prediction.

## Acknowledgements
- Dataset: PIMA Diabetes dataset.
- References: Research and documentation provided in the project.
