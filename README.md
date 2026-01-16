# Cardiovascular Risk Prediction: A Clinical Data Analysis 🫀

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Machine_Learning-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Project-Portfolio-success)

## Project Overview
This project focuses on predicting the presence of heart disease using clinical features from the UCI Heart Disease dataset. Beyond simple classification, this project explores the **medical significance** of specific biomarkers like ST Depression (`oldpeak`) and Maximum Heart Rate (`thalach`).

The goal is to provide a transparent, interpretable model that could assist clinicians in identifying high-risk patients.

## Clinical Insights & Key Features
Before modeling, I conducted an Exploratory Data Analysis (EDA) to understand the "Medical Red Flags" in the data:
* **ST Depression (oldpeak):** Patients with heart disease showed significantly higher levels of ST depression during stress tests.
* **Vascular Health (ca):** The number of major vessels colored by fluoroscopy emerged as a top predictor.
* **Heart Rate (thalach):** A lower maximum heart rate during physical activity was strongly correlated with disease presence.

## Technical Workflow
1.  **Data Cleaning:** Handled missing values (encoded as `?` in raw data) and converted the multi-class target into a binary classification task.
2.  **Feature Engineering:** Applied **One-Hot Encoding** to categorical variables (`cp`, `thal`, `slope`) and **Standard Scaling** to numeric features to ensure model convergence.
3.  **Modeling:** Implemented **Logistic Regression** to maintain high model interpretability.
4.  **Evaluation:** Focused on **Recall** and the **Confusion Matrix** to ensure the model minimizes "False Negatives" (missed sick patients).

## Results & Visualizations
*(Note: Replace the placeholder below with the link to the image you saved!)*

### Feature Importance (The "Red Flags")
![Feature Importance](portfolio_images/feature_importance.png)
*Figure 1: Logistic Regression coefficients showing which clinical factors most influence the prediction.*

## How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/bamideleadedeji/heart-disease-prediction.git


2.  Install dependency:
     pip install pandas seaborn scikit-learn matplotlib ucimlrepo

3   Run the Jupyter Notebook heart_disease_analysis.ipynb

Repository Structure
heart_disease_analysis.ipynb: The complete step-by-step analysis.
portfolio_images/: Saved visualizations for the report.
heart_disease_cleaned.csv: The processed dataset ready for ML.
Conclusion
This project demonstrates that while accuracy is important, interpretability in medical AI is vital. 
By identifying which features (like oldpeak) drive predictions, we bridge the gap between "Black Box" algorithms and 
actionable clinical insights. Future iterations of this project could incorporate a Cost-Sensitive Learning approach, 
where the penalty for missing a heart disease case is weighted more heavily than a false alarm
Author: Adedeji Bamidele
Connect: www.linkedin.com/in/adedeji-bamidele-88a159263 | bamideleadedeji2000@gmail.com
