# Cirrhosis Patient Outcome Prediction

## Overview
Cirrhosis is a severe liver disease that can lead to critical health complications. Predicting patient outcomes can significantly aid in early interventions, healthcare strategies, and treatment planning. This project aims to develop a multi-class classification model to predict the outcomes of cirrhosis patients based on demographic, clinical, and health-related features.


## Installation
To set up the project locally, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/OmidMahdawi/Classification-Model.git
   cd Classification-Model
   ```


## Data Preprocessing
- Missing values are handled using median imputation for numerical variables and the most frequent value for categorical variables.
- Categorical variables are encoded using `LabelEncoder`.
- Features are standardized using `StandardScaler` to improve model performance.

## Model Training
The following machine learning models are trained and evaluated:
- **Logistic Regression**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **XGBoost Classifier** (Best-performing model)

The model is trained on a stratified train-test split (80-20) and evaluated using:
- **Accuracy**
- **F1 Score (Macro)**
- **ROC-AUC Score**
- **Confusion Matrix**

## Prediction Output Format
For each row in the test set, the model predicts the probability of each outcome:
```
id,Status_C,Status_CL,Status_D
7905,0.628084,0.034788,0.337128
7906,0.628084,0.034788,0.337128
7907,0.628084,0.034788,0.337128
```

## Exploratory Data Analysis (EDA)
Key data analysis steps include:
- Summary statistics & missing value detection
- Feature distributions (histograms, KDE plots)
- Correlation analysis (heatmaps, pairplots)
- Outlier detection and handling



## Future Improvements
- **Hyperparameter tuning** for improved model performance
- **Advanced feature engineering** for better predictive power
- **Deploying the model** as an API for real-time predictions

## Contributions
Contributions are welcome! If you'd like to enhance the project, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For inquiries, please contact: `omidmahdawi100@gmail.com`
