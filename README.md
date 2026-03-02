# BMB433 Helicase Activity Prediction

This repository contains a Python project that predicts the biological activity of molecules against Helicase targets using a Support Vector Machine (SVM) model. The project covers data preprocessing, visualization, model training, and evaluation.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

The main objective of this project is to predict compound activity (Active/Inactive) by performing the following steps:

**Preprocessing:**
* Fill missing values in numerical features using the mean strategy.
* Convert categorical "Outcome" features to numerical values using label encoding.
* Normalize feature distributions using Standard Scaling.

**Visualization:**
* Generate and save a confusion matrix heatmap to visualize prediction errors.

**Modeling:**
* Train a Support Vector Classifier (SVC) with an RBF kernel.
* Evaluate model performance using Accuracy and Weighted F1-Score.

## Dataset

The project uses bioactivity data derived from the ChEMBL database.
Please ensure the dataset file (`heli-smacc (1).csv`) is placed in the root directory or update the file path in the script accordingly.

## Installation

Clone the repository and install the required packages. It is recommended to use a virtual environment.

```bash
# Clone the repository
git clone [https://github.com/yourusername/BMB433-Project.git](https://github.com/yourusername/BMB433-Project.git)
cd BMB433-Project

# (Optional) Create and activate a virtual environment
python -m venv venv

# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install numpy pandas seaborn matplotlib scikit-learn


Usage
To run the project, execute the main script (or run the Jupyter Notebook):

Bash
python main.py
Note: If using the Jupyter Notebook (Copy_of_BMB433.ipynb), simply open it in Jupyter Lab or Google Colab and run all cells.

Project Structure
Plaintext
├── heli-smacc (1).csv      # Dataset file
├── main.py                 # Main script (or Copy_of_BMB433.ipynb)
├── confusion_matrix.png    # Output visualization (generated after running)
├── README.md               # Project documentation
└── requirements.txt        # List of dependencies
Results
The model outputs the following metrics upon execution:

Accuracy Score

F1 Score

Confusion Matrix Plot (Saved as confusion_matrix.png)

Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements.

License
This project is open-source and available for educational purposes.
