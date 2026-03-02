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
