# 🚢 Task 01 — Titanic Classification

## 📌 Objective
Predict whether a passenger survived the Titanic disaster using features like age, gender, passenger class, and family size.

---

## 📂 Files

| File | Description |
|------|-------------|
| `Task01_The_Titanic_Clasification.ipynb` | Main notebook with full analysis and model |
| `train.csv` | Training dataset |
| `test.csv` | Test dataset |
| `gender_submission.csv` | Sample submission file |
| `cleaned_titanic.csv` | Cleaned/preprocessed dataset |
| `Titanic_Classification_Report_Rhombix.docx` | Full project report |

---

## 🔍 Steps Covered

1. **Load Dataset** — Loaded directly via Seaborn's built-in Titanic dataset
2. **Exploratory Data Analysis (EDA)**
   - Survival rate by sex
   - Survival rate by passenger class
   - Age distribution by survival
   - Correlation heatmap
3. **Data Preprocessing** — Handled missing values, encoded categorical features, scaled numerical features
4. **Model Training** — Logistic Regression & Random Forest Classifier
5. **Evaluation** — Accuracy, confusion matrix, classification report, cross-validation

---

## 📊 Key Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | ~80% |
| Random Forest | ~82% |

---

## 🛠️ Libraries Used

- `pandas`, `numpy`
- `seaborn`, `matplotlib`
- `scikit-learn`

---

## 👤 Author

**Usman Nazir** — Data Science Intern @ Rhombix Technologies
