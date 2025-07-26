# PLAICraft-Project
# Predicting Game Newsletter Subscription Using KNN Classification

This project explores how player characteristics—specifically **age** and **playtime**—influence the likelihood of subscribing to a game-related newsletter. The analysis was conducted in **R** using a dataset provided through a university course. 

We applied **data wrangling**, **exploratory data analysis (EDA)**, and **K-Nearest Neighbours (KNN)** classification to build a predictive model and evaluate player behavior trends.

## 📊 Objective
To answer the question:
> _How does age and play time predict the likelihood of an individual subscribing to a game-related newsletter?_

## 🧪 Methods

- **Data Cleaning:** Selected relevant variables (`Age`, `played_hours`, `subscribe`) and handled missing values using mean imputation.
- **EDA & Visualization:** Created grouped bar plots and a scatterplot to examine relationships between variables.
- **Modeling:** Used `tidymodels` to implement a **KNN classifier** with standardized features and upsampling to address class imbalance.
- **Tuning:** Evaluated K values from 1 to 40 using 5-fold cross-validation.
- **Evaluation Metrics:** Accuracy, Precision, Recall, and Confusion Matrix.

## 🔍 Key Findings

- **Average player age**: early 20s  
- **Average playtime**: ~5 hours  
- **Most subscribers** were aged 15–25 with higher playtimes
- KNN model achieved:
  - **Accuracy:** 49%
  - **Precision:** 87%
  - **Recall:** 36%

These results indicate that while the model is highly selective (high precision), it struggles with recall—missing many true subscriber cases due to feature overlap between groups.

## 🧠 Discussion

The overlap in age and playtime distributions between subscribers and non-subscribers likely limited model performance. While clear trends emerged during EDA, the final model's accuracy suggests that **additional features** (e.g., gender, session frequency, experience level) may be necessary to improve predictive power.

## 🛠 Tools Used

- R  
- tidyverse  
- tidymodels  
- ggplot2  
- JupyterLab (R kernel)
