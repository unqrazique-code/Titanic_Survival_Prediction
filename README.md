#  Titanic Survival Prediction

##  Project Overview

This project builds a machine learning model to predict whether a passenger survived the Titanic disaster. It demonstrates a complete data science workflow including data cleaning, exploratory analysis, feature engineering, and model building.

---

##  Problem Statement

Given passenger details such as age, gender, class, and fare, predict whether the passenger survived (1) or not (0).

---

##  Dataset Files

| File Name              | Description                                            |
| ---------------------- | ------------------------------------------------------ |
| train.csv            | Training dataset (includes target variable Survived) |
| test.csv             | Test dataset (no target column)                        |
| submission.csv       | Final prediction output file                           |
| train-checkpoint.csv | Backup file (auto-generated)                           |

---

##  Dataset Features

* **PassengerId** – Unique identifier
* **Survived** – Target variable (0 = No, 1 = Yes)
* **Pclass** – Passenger class (1, 2, 3)
* **Name** – Passenger name
* **Sex** – Gender
* **Age** – Age
* **SibSp** – Siblings/Spouses aboard
* **Parch** – Parents/Children aboard
* **Ticket** – Ticket number
* **Fare** – Ticket fare
* **Cabin** – Cabin number
* **Embarked** – Port of embarkation

---

##  Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

##  Project Workflow

###  1. Data Cleaning

* Filled missing values (Age, Embarked)
* Dropped irrelevant columns (Cabin, Name, Ticket)

###  2. Feature Engineering

* Converted categorical variables:

  * Sex → numeric (0,1)
  * Embarked → one-hot encoding
* Created new features (optional):

  * Family size

###  3. Exploratory Data Analysis (EDA)

* Survival distribution by gender
* Survival vs passenger class
* Correlation heatmap

###  4. Model Building

Models used:

* Logistic Regression (baseline)
* Decision Tree (improvement)

###  5. Model Evaluation

* Accuracy Score
* Confusion Matrix

---

##  Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | ~78–82%  |
| Decision Tree       | ~75–85%  |

---

##  Kaggle Score

**Public Leaderboard Score: 0.73205**

This score represents the model's prediction accuracy on unseen test data submitted to Kaggle. It reflects a solid beginner-level performance and a good understanding of data preprocessing and basic machine learning techniques.

---

##  Key Insights

*  Females had significantly higher survival rates
*  First-class passengers survived more
*  Higher fare correlated with survival
*  Children had better survival chances

---

##  Project Screenshots

###  Data Overview

![Data Overview]()

###  Missing Values Handling

* Missing Values in Train

![Missing Value in Train](https://github.com/unqrazique-code/Titanic_Survival_Prediction/blob/9b2cecc28b8de4048197642a3feadd6f2e5bb03b/missing%20values%20in%20train.png)

* Missing Value in Test

![Missing Value in Test](https://github.com/unqrazique-code/Titanic_Survival_Prediction/blob/9b2cecc28b8de4048197642a3feadd6f2e5bb03b/missing%20values%20in%20Test.png)

###  EDA Visualization

* Survival by Gender

  ![Survival by Gender](https://github.com/unqrazique-code/Titanic_Survival_Prediction/blob/9b2cecc28b8de4048197642a3feadd6f2e5bb03b/survival%20by%20Gender.png)

* Survival by Class

  ![Survival by Class](https://github.com/unqrazique-code/Titanic_Survival_Prediction/blob/9b2cecc28b8de4048197642a3feadd6f2e5bb03b/survival%20by%20Class.png)

###  Model Training

![Model Training](https://github.com/unqrazique-code/Titanic_Survival_Prediction/blob/9b2cecc28b8de4048197642a3feadd6f2e5bb03b/model%20training.png)

###  Model Evaluation

![Model Evaluation]()

---

##  How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook
```

Open the notebook and run all cells step by step.

---

##  Output

* Cleaned dataset
* Trained ML model
* Predictions file (`submission.csv`)

---

##  Future Improvements

* Hyperparameter tuning
* Random Forest / XGBoost
* Advanced feature engineering
* Model deployment (Streamlit / Flask)

---

## ⭐ Final Note

This project is a foundational step into data science and machine learning. It focuses on building intuition, not just accuracy.

---
