<div align="center">

# 🚢 Titanic Survival Classification

### Rhombix Technologies — Data Science Internship | Task 01

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas)](https://pandas.pydata.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org)

</div>

---

## 📌 Problem Statement

On **April 15, 1912**, the RMS Titanic sank after colliding with an iceberg.  
Of **2,224 passengers and crew**, only **710 survived**.

**Task:** Build a binary classification model to predict whether a passenger survived (`1`) or did not survive (`0`) based on features like gender, age, ticket class, and fare.

---

## 🗂️ Steps Performed

**1. Data Loading & Inspection**
- Loaded `train.csv` (891 rows), `test.csv` (418 rows), `gender_submission.csv`
- Checked shape, data types, and missing value counts

**2. Exploratory Data Analysis (EDA)**
- Survival rate by gender → females: ~74%, males: ~19%
- Survival rate by class → 1st: 63%, 2nd: 47%, 3rd: 24%
- Age distribution → children had higher survival rates
- Fare analysis → higher fare strongly linked to survival
- Embarkation port → Cherbourg passengers survived most (~55%)
- Family size → small families (2–4) survived best

**3. Feature Engineering**
- Created `FamilySize` = `SibSp` + `Parch` + 1
- Extracted passenger titles from `Name`
- Binned `Age` and `Fare` into categories

**4. Data Preprocessing**
- Imputed missing `Age` values with median
- Imputed missing `Embarked` with mode
- Dropped `Cabin` (>77% missing)
- Label encoded categorical features (`Sex`, `Embarked`)
- Scaled numeric features with `StandardScaler`

**5. Model Training**
- Split train data: 80% train / 20% validation
- Trained 3 models: Logistic Regression, Random Forest, Gradient Boosting

**6. Model Evaluation**
- Evaluated using accuracy, confusion matrix, classification report
- Used 5-fold cross-validation for robust scoring

---

## 🤖 Models & Results

| Model | Validation Accuracy | CV Score (5-fold) |
|-------|--------------------|--------------------|
| Logistic Regression | ~80% | ~79% |
| Random Forest Classifier | ~83% | ~82% |
| **Gradient Boosting Classifier** | **~84%** | **~83%** |

**Best Model: Gradient Boosting Classifier — ~84% accuracy**

### 📊 Interpretation
- **Gender** was the single strongest predictor of survival
- **Pclass** and **Fare** were the top numeric predictors
- Gradient Boosting outperformed other models by capturing non-linear feature interactions
- The model correctly identifies ~84 out of every 100 passengers' survival outcome

---

## 📂 Files

| File | Description |
|------|-------------|
| `notebook.ipynb` | Full analysis — EDA, preprocessing, training, evaluation |
| `train.csv` | Training data (891 labeled rows) |
| `test.csv` | Test data (418 unlabeled rows) |
| `gender_submission.csv` | Sample submission format |
| `requirements.txt` | Python dependencies |
| `Titanic_Classification_Report_Rhombix.docx` | Full project report |

---

## ⚙️ Run Locally

```bash
git clone https://github.com/realusmannazir1/RhombixTechnologies_Tasks.git
cd RhombixTechnologies_Tasks/Titanic_Classification

pip install -r requirements.txt
jupyter notebook notebook.ipynb
```

---

## 👤 Author

**Usman Nazir** — Data Science Intern @ Rhombix Technologies  
[GitHub](https://github.com/realusmannazir1)
