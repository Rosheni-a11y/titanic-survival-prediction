# Titanic Survival Prediction

## Overview
This project predicts passenger survival on the Titanic using machine learning techniques. It was developed as a beginner-friendly data science project based on the Kaggle Titanic competition, focusing on data preprocessing, feature engineering, and model evaluation.

---

## Results
- **Best Model:** Random Forest Classifier  
- **Validation Accuracy:** 81.56%  
- **Kaggle Public Score:** 0.75598  
- **Leaderboard Position:** Top 50%  

---

## Technologies Used
- Python
- Pandas - Data manipulation
- NumPy - Numerical computing
- Scikit-learn - Machine learning models
- Matplotlib & Seaborn - Data visualization
- Google Colab - Development environment

---

## Dataset
The dataset is obtained from the **Kaggle Titanic Machine Learning Competition** (https://www.kaggle.com/c/titanic).

**Key Features Used**
- Passenger Class (Pclass)
- Sex
- Age
- Fare
- Siblings/Spouses (SibSp)
- Parents/Children (Parch)
- Embarked
- Engineered Features: FamilySize, IsAlone

---

## Methodology

### 1. Data Exploration
- Analyzed 891 training passengers
- Visualized survival rates by gender, class, age
- Identified missing values (Age, Cabin, Embarked)

### 2. Data Preprocessing
- Handled missing values (median imputation for Age)
- Feature engineering: Created FamilySize and IsAlone features
- Encoded categorical variables (Sex, Embarked)
- Standardized numerical features

### 3. Model Training
Trained and compared multiple models:
- **Logistic Regression:** 80.45% validation accuracy, AUC: 0.8513
- **Random Forest:** 81.56% validation accuracy, AUC: 0.8316

### 4. Evaluation
- Confusion matrix analysis
- ROC curve and AUC scores
- Classification reports (precision, recall, F1-score

---

## Key Insights
**Most Important Features for Survival:** 
1. **Sex** (0.54 correlation) - Women had 74% survival rate vs men's 19% 
2. **Pclass** (-0.34 correlation) - 1st class: 63% survival, 3rd class: 24%
3. **Fare** (0.26 correlation) - Higher fare = better survival chances
   
**Model Performance:** 
-Successfully predicted 75.6% of test passengers correctly 
-Best at identifying deaths (87% recall)
-Room for improvement in catching survivors (72% recall)

---

## Project Structure

```

titanic-survival-prediction/
│
├── titanic_machine_learning.ipynb
├── titanic_submission.csv
├── README.md

```
---

## What I Learned
- Data preprocessing and handling missing values
- Feature engineering techniques
- Training and evaluating ML models
- Dealing with overfitting
- The importance of validation strategies
- How to create Kaggle submissions

---

## Future Improvements

- [ ] Implement cross-validation for better estimates
- [ ] Try ensemble methods (XGBoost, Gradient Boosting)
- [ ] Extract more features from Name column (titles: Mr, Mrs, Master)
- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Feature selection to reduce overfitting
- [ ] Try neural networks

---

## Author
**Rosheni Bolonne**  
Artificial Intelligence Undergraduate
