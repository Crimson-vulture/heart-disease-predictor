# Heart Disease Prediction Using Machine Learning

An end-to-end Machine Learning project that analyzes clinical and cardiovascular features to predict the presence or absence of heart disease using classification algorithms. The project includes data cleaning, exploratory data analysis, preprocessing, model comparison, and an interactive Streamlit web application.

## Overview

This project uses a heart disease dataset containing demographic information, cardiovascular measurements, and exercise-related indicators to build a machine learning classification system.

The dataset is explored and cleaned before applying feature preprocessing and scaling. Multiple classification algorithms are trained and evaluated using metrics such as accuracy, precision, recall, and F1-score.

The trained model and necessary preprocessing artifacts are saved using Pickle and integrated into a Streamlit application, allowing users to enter patient-related features and obtain a model prediction.

The target variable is `HeartDisease`, which represents the presence or absence of heart disease according to the dataset's labeling convention.

## Dataset Features

The dataset contains the following 12 columns:

| Feature | Description |
|---|---|
| `Age` | Age of the individual |
| `Sex` | Sex category recorded in the dataset |
| `ChestPainType` | Type of chest pain |
| `RestingBP` | Resting blood pressure |
| `Cholesterol` | Serum cholesterol level |
| `FastingBS` | Fasting blood sugar indicator |
| `RestingECG` | Resting electrocardiogram results |
| `MaxHR` | Maximum heart rate achieved |
| `ExerciseAngina` | Whether exercise-induced angina is present |
| `Oldpeak` | ST depression induced by exercise relative to rest |
| `ST_Slope` | Slope of the peak exercise ST segment |
| `HeartDisease` | Target variable indicating the dataset's heart disease label |

**Target variable:** `HeartDisease`

The input features are used to predict the target label. The target column should not be included among the model's input features.

## Project Workflow

1. **Data Inspection and Cleaning:** Examining the dataset, identifying data quality issues, and handling missing values or duplicates where appropriate.
2. **Exploratory Data Analysis:** Investigating feature distributions, correlations, and relationships with the target variable.
3. **Data Preprocessing:** Encoding categorical features, preparing numerical features, and applying feature scaling where required.
4. **Model Training:** Training multiple classification algorithms to learn patterns in the data.
5. **Model Evaluation:** Comparing models using accuracy, precision, recall, and F1-score.
6. **Model Persistence:** Saving the selected trained model and required preprocessing objects using Pickle.
7. **Application Development:** Building an interactive Streamlit interface for entering feature values and generating predictions.

## Tech Stack

- **Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, sheryanalysis
- **Machine Learning:** Scikit-learn
- **Development:** Jupyter Notebook, Visual Studio Code
- **Web Application:** Streamlit
- **Model Persistence:** Pickle

## Model Evaluation

Multiple classification algorithms were trained and compared using the following metrics:

- **Accuracy:** Overall proportion of correctly classified observations.
- **Precision:** Proportion of positive predictions that were correct.
- **Recall:** Proportion of actual positive cases correctly identified.
- **F1-score:** Harmonic mean of precision and recall.

The model comparison results are used to assess predictive performance and select a suitable model for the application.

*Insert the actual evaluation results from the notebook here. Performance should be assessed on data not used for model training.*

## Streamlit Web Application

The application provides an interactive interface for entering cardiovascular and demographic features. It loads the saved machine learning model and the required preprocessing artifacts to generate a prediction.

The interface displays the predicted class according to the model's output and the target definition used in the dataset.

**Live application:** Add the deployed Streamlit URL here.

## Installation and Usage

### 1. Clone the repository

```bash
git clone https://github.com/Crimson-vulture/heart-disease-predictor.git
cd heart-disease-predictor
```

### 2. Create and activate a virtual environment

```bash
python -m venv .venv
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the application

```bash
streamlit run app/app.py
```

Ensure that all saved model and preprocessing files are available at the paths expected by the application.

## Limitations and Disclaimer

This project is intended for educational and machine learning demonstration purposes.

The model predicts the dataset-defined heart disease label. It does not establish an individual's future probability of developing heart disease, predict stroke risk, or provide a clinically validated diagnosis.

Predictions depend on the training data, selected features, preprocessing methods, and model performance. The application should not be used as a substitute for medical advice, diagnosis, or treatment.

## Dataset Source

Add the original dataset source, attribution, and applicable license information here.

## Author

ADITYA

- GitHub: https://github.com/Crimson-vulture
- LinkedIn: www.linkedin.com/in/crimson-vulture

