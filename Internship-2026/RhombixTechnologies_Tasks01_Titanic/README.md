# 🚢 Titanic Survival Classification

> **Rhombix Technologies — Data Science Internship | Task 01**

Predict whether a passenger survived the Titanic disaster using machine learning — based on features like age, gender, ticket class, and fare.

---

## 📌 Problem Statement

On **April 15, 1912**, the RMS Titanic sank after hitting an iceberg.  
Of **2,224 passengers and crew**, only **710 survived**.

**Goal:** Build a binary classification model to predict survival (`1 = Survived`, `0 = Did Not Survive`) using passenger data.

---

## 📂 Project Structure

```
RhombixTechnologies_Tasks01_Titanic/
├── RhombixTechnologies_Tasks01.ipynb   # Main notebook
├── train.csv                           # Training data (891 rows, labeled)
├── test.csv                            # Test data (418 rows, unlabeled)
├── gender_submission.csv               # Sample submission format
└── README.md
```

---

## 📊 Dataset

| Column | Description |
|--------|-------------|
| `PassengerId` | Unique passenger ID |
| `Survived` | Target: 0 = No, 1 = Yes |
| `Pclass` | Ticket class (1st / 2nd / 3rd) |
| `Name` | Passenger name |
| `Sex` | Gender |
| `Age` | Age in years |
| `SibSp` | # of siblings/spouses aboard |
| `Parch` | # of parents/children aboard |
| `Ticket` | Ticket number |
| `Fare` | Passenger fare |
| `Cabin` | Cabin number |
| `Embarked` | Port: C = Cherbourg, Q = Queenstown, S = Southampton |

---

## 🗂️ Notebook Walkthrough

| Step | Section |
|------|---------|
| 1 | 📦 Import Libraries |
| 2 | 📥 Load Data |
| 3 | 🔍 Exploratory Data Analysis (EDA) |
| 4 | 📊 Data Visualization |
| 5 | ⚙️ Feature Engineering |
| 6 | 🧹 Data Preprocessing |
| 7 | 🤖 Model Training |
| 8 | 📈 Model Evaluation |
| 9 | 🏆 Feature Importance |
| 10 | 🔮 Predictions & Submission |
| 11 | ✅ Conclusion |

---

## 🤖 Models Used

- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

---

## 🔑 Key Insights

- **Gender** was the strongest predictor — females had much higher survival rates
- **Pclass** mattered — 1st class passengers survived more
- **Age** played a role — children were prioritized
- **Family size** had a non-linear effect on survival

---

## ⚙️ Setup & Run

```bash
# Clone the repo
git clone https://github.com/realusmannazir1/RhombixTechnologies_Tasks01_Titanic.git
cd RhombixTechnologies_Tasks01_Titanic

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch notebook
jupyter notebook RhombixTechnologies_Tasks01.ipynb
```

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 👤 Author

**Usman Nazir**  
Data Science Intern @ Rhombix Technologies  
[GitHub](https://github.com/realusmannazir1)

---

## 📄 License

This project is for educational and internship purposes.
