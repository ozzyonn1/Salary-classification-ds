# Salary Classification in Data Science

This project focuses on predicting salary categories in the Data Science field using supervised machine learning models.  
The dataset includes job-related features such as **job title**, **experience level**, **work setting** (remote/on-site), **company size**, and **employee residence**.

The project was completed as part of the course *Metody Walidacji Modeli Statystycznych* at Lublin University of Technology (2025).

---

## Project Objective

The goal was to build and validate multiple classification models to predict whether a given job's salary is:
- **Below average**
- **Average**
- **Above average**

We performed preprocessing, feature selection, model comparison, and final evaluation based on classification metrics.

---

## Repository Contents

- `Metody_walidacji.html` – Final report with visualizations and model summaries  
- `Cleaned_Dataset.csv` – Cleaned dataset used in modeling *(optional)*  
- `README.md` – This project description

---

## Workflow Overview

1. **Data Cleaning**
   - Removed outliers and missing values
   - Standardized salary values and created a new categorical target variable

2. **Feature Engineering**
   - Encoding categorical variables (`job_title`, `company_size`, etc.)
   - Scaling numerical variables using `StandardScaler`

3. **Model Training**
   - Used multiple classifiers:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - Support Vector Machine (SVM)
     - k-Nearest Neighbors (k-NN)
   - Applied feature selection with `SelectKBest` using mutual information

4. **Model Validation**
   - Performed 10-fold cross-validation
   - Evaluated using:
     - Accuracy
     - Precision
     - Recall
     - F1-score
     - Confusion Matrix

5. **Final Model**
   - The **Random Forest Classifier** showed the best performance with balanced precision and recall across salary classes.

---

## Tools & Libraries Used

- `R` (tidymodels, caret, ggplot2)
- `dplyr`, `tidyr`, `readr`, `stringr`
- `e1071`, `randomForest`, `class`, `nnet`
- RMarkdown / HTML export for reporting

---

## Key Insights

- Salary level correlates strongly with **experience level** and **company size**
- **Remote work** does not guarantee higher salaries in all cases
- Feature selection improved model stability and interpretability


---

## Author

**Oleh Zemlianyi**  
Politechnika Lubelska | Data Engineering & Analytics  
[LinkedIn Profile](https://www.linkedin.com/in/oleh-zemlianyi)  

