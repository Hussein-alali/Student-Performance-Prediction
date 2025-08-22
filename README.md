# 📚 Student Performance Prediction

## 📌 Project Overview
This project predicts student performance scores based on study-related features such as **Hours Studied, Attendance, and Previous Scores**.  
We compare **Linear Regression** with **Polynomial Regression** using **5-Fold Cross-Validation** to evaluate how well each model fits the data.

---

## 🚀 Key Highlights
- **Goal:** Predict student performance (regression task).  
- **Dataset:** Student performance dataset (Hours_Studied, Attendance, Previous_Scores, etc.).  
- **Feature Scaling:** Applied **StandardScaler** for numerical features.  
- **Models Used:**  
  - Linear Regression (baseline).  
  - Polynomial Regression (degree=2).  
- **Evaluation Metric:** R² Score (Coefficient of Determination).  
- **Cross-Validation:** Used **KFold (5 splits, shuffle=True)** for robust evaluation.  

---

## 📊 Performance Results
| **Model**              | **Fold R² Scores**                                       | **Mean R² Score** |
|-------------------------|----------------------------------------------------------|-------------------|
| Linear Regression       | [0.9656, 0.9641, 0.9622, 0.9688, 0.9695]                 | **0.9660**        |
| Polynomial Regression   | [0.9652, 0.9638, 0.9622, 0.9679, 0.9690]                 | **0.9656**        |

✅ Both models perform almost identically, with **Linear Regression slightly higher** on average.  
✅ Polynomial Regression does not provide a clear improvement for this dataset.  

---

## 🛠 Tools & Libraries
- **Python**  
- **NumPy, Pandas**  
- **Scikit-learn** (LinearRegression, PolynomialFeatures, StandardScaler, Pipeline, KFold, cross_val_score)  
- **Matplotlib, Seaborn** (visualizations and EDA)  

---

## 📈 Workflow
1. **Data Preprocessing:**  
   - Selected numeric columns for scaling (`Hours_Studied, Attendance, Previous_Scores`).  
   - Standardized features with **StandardScaler**.  
2. **EDA (Exploratory Data Analysis):**  
   - Checked missing values and outliers.  
   - Plotted distributions and correlations.  
3. **Model Training:**  
   - Built **Linear Regression Pipeline**.  
   - Built **Polynomial Regression Pipeline** (degree=2).  
4. **Model Evaluation:**  
   - Applied **5-Fold Cross-Validation**.  
   - Compared R² scores across folds and calculated mean.  

---

## 🧩 How to Run
1. Clone the repository:

    git clone https://github.com/Hussein-alali/Student-Performance-Prediction.git

2. Install dependencies:

    pip install -r requirements.txt

3. Run The Notebook:

    jupyter notebook Student_Performance_Prediction.ipynb

---

## 📘 License
This project is licensed for educational and personal use.

---

## 🙋 Author
**Hussein Abdalrhman Alali Alhlal**  
Computer Engineer | Data & AI Enthusiast

---
