Breast Tissue Classification using Impedance Measurements
Project Overview-

This project focuses on Breast Tissue Classification using electrical impedance measurement features. The objective is to classify different types of breast tissue based on biomedical signal characteristics using a Machine Learning approach.

A complete Scikit-learn pipeline was implemented including:

Missing value imputation

Feature scaling

Random Forest classification

The model achieved:

Test Accuracy: 77.27%

Best Cross-Validation Score: 0.6316

Dataset Information

The dataset contains impedance measurement features extracted from breast tissue samples.

🔹 Features Used
X = df[['I0', 'PA500', 'HFS', 'Area', 'DA', 'DR']]
y = df['Class']

Feature	Description
I0	Impedance at zero frequency
PA500	Phase angle at 500 kHz
HFS	High-frequency slope
Area	Area under impedance spectrum
DA	Distance between spectral curves
DR	Ratio of distances

Target Variable:

Class → Type of breast tissue

Technologies Used-

Python

NumPy

Pandas

Scikit-learn

Matplotlib (for visualization)

Machine Learning Pipeline

The model was built using a Scikit-learn Pipeline:-
from sklearn.pipeline import Pipeline
from sklearn.impute import SimpleImputer
from sklearn.preprocessing import StandardScaler
from sklearn.ensemble import RandomForestClassifier

pipeline = Pipeline([
    ('imputer', SimpleImputer()),
    ('scaler', StandardScaler()),
    ('model', RandomForestClassifier())
])

Pipeline Steps-

SimpleImputer – Handles missing values

StandardScaler – Normalizes feature values

RandomForestClassifier – Performs classification

Model Performance-
Metric	Score
Test Accuracy	0.7727
Best Cross-Validation Score	0.6316

Cross-validation was used to ensure model generalization and reduce overfitting.

How to Run the Project-
1️ Clone the Repository
[git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name]

2️ Install Dependencies
[pip install -r requirements.txt]

3️ Run the Notebook or Script
[python main.py]

or open the Jupyter Notebook.
