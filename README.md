BMB433: Helicase Activity Prediction
Project Overview
This project utilizes machine learning techniques to predict the biological activity of molecules against Helicase targets (specifically SUV3 Helicase and NS3 Helicase/NTPase). Using data derived from the ChEMBL database, the goal is to classify compounds as "Active" or "Inactive" based on their molecular properties and assay results.

Dataset
The dataset (heli-smacc (1).csv) includes bioactivity data for over 20,000 compounds. Key features analyzed include:

Molecular Weight

Standard Value (IC50)

Outcomes (Active vs. Inactive classification)

Methodology
The project implements a supervised learning pipeline in Python:

Data Preprocessing: Handling missing values using SimpleImputer and encoding categorical outcomes.

Feature Scaling: Normalizing feature distributions using StandardScaler.

Modeling: Training a Support Vector Classifier (SVC) to predict compound activity.

Evaluation: Assessing model performance using Accuracy, F1-Score, and Confusion Matrix visualization.

Technologies Used
Python 3

Pandas & NumPy (Data Manipulation)

Scikit-Learn (Machine Learning & Metrics)

Seaborn & Matplotlib (Data Visualization)
