# Smartphone Sensor Activity Recognition (HAR)

![Python](https://img.shields.io/badge/Python-3.10-blue)  
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.7-brightgreen)  
![Status](https://img.shields.io/badge/Status-Completed-success)

This project focuses on building a machine learning pipeline to classify five fundamental human activities using smartphone sensor data. The data was collected with the **Sensor Logger** app (iOS/Android), recording accelerometer, gyroscope, and gravity readings at 100 Hz. Each activity was performed multiple times with consistent smartphone placement in a tight pocket to ensure reproducibility.

This project demonstrates how smartphone sensors can be leveraged for real-time human activity recognition — a key capability in areas such as **fitness tracking**, **digital health monitoring**, and **context-aware computing**.

The dataset covers the following activities: **sitting down**, **standing up**, **walking**, **running**, and **climbing stairs**. Each file follows a consistent naming scheme, for example:  
`P01_Walk_20251009_0.csv` → Person 1, first walking trial, collected on October 9 2025.  
This structure provides clear information about the participant, activity type, recording date, and repetition number.

After preprocessing and feature engineering, several supervised learning models were trained and evaluated, including **Logistic Regression**, **Decision Tree**, **Random Forest**, **Gaussian Naive Bayes**, and **K-Nearest Neighbors**. Model performance was assessed using **Accuracy**, **F1-Score**, and **Cohen’s Kappa**, supported by confusion matrices and class-wise precision/recall metrics.

Among all evaluated models, **Logistic Regression** and **K-Nearest Neighbors** achieved the highest accuracy (≈ 98 %), showing that even simple, well-regularized models can effectively capture motion patterns from sensor data. Further improvements could be achieved through **hyperparameter tuning**, **larger and more diverse datasets**, and **additional engineered features** that better describe temporal and spatial movement dynamics.

---

### ⚙️ Setup

Clone the repository and install the required dependencies:  
`git clone https://github.com/FinnS17/smartphone-sensor-activity-recognition.git`  
`cd smartphone-sensor-activity-recognition`

Install dependencies:  
- Python 3.10.18  
- numpy 2.0.1  
- pandas 2.3.2  
- matplotlib 3.10.5  
- seaborn 0.13.2  
- scikit-learn 1.7.1  
- scipy 1.15.3  

Then open the notebook and run all cells:  
`jupyter notebook activity_recognition_pipeline.ipynb`

---

### 📁 Project Structure

- **data/** – raw sensor data
- **activity_recognition_pipeline.ipynb** – main analysis notebook  
- **README.md** – project overview and setup guide  

---

*Author: Finn Stäcker*  
*Year: 2025*