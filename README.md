# Enhancing-Patient-Triage
This project enhances Montanaro Hospital's OU efficiency. It uses data analytics and predictive models (Random Forest best) to identify factors (temp, BP, age, diagnosis) causing patient "flips" from observation to inpatient. The goal is to optimize patient triage and improve resource utilization.
Sure, here's a README for your GitHub project:

# 🏥 Enhancing Patient Triage Efficiency in Montanaro Hospital's Observation Unit

## 📊 Project Overview
This project addresses operational inefficiencies in Montanaro Hospital's 23-bed Observation Unit (OU), where a significant number of patients initially admitted for observation are later transitioned ("flipped") to inpatient status. The goal was to identify key predictors of patient flips and develop a machine learning model to support data-driven triage decisions.

---

## 🎯 Objectives
- Analyze clinical and demographic data to uncover flip patterns.
- Build predictive models to forecast the likelihood of a patient flipping to inpatient status.
- Recommend triage process improvements based on data insights.

---

## 📁 Dataset
- **Size**: 1,111 patient records
- **Variables**: 17 features including age, blood pressure, temperature, diagnosis group, and OU length of stay.
- **Target Variable**: `Flipped` (1 = flipped to inpatient, 0 = stayed in OU)

---

## 🧪 Techniques Used
- **Descriptive Analytics**
- **Logistic Regression**
- **Random Forest**
- **Decision Tree**
- **Data Cleaning and Feature Engineering**
- **Model Evaluation Metrics**: Accuracy, AUC, Sensitivity, Specificity, RMSE, MAE

---

## 🧠 Key Findings
- **High Flip Rate**: 53.9% of patients flipped to inpatient status.
- **Top Risk Factors**:
  - Normal temperature (not a reliable indicator of short stay)
  - Prehypertension and mild hypertension
  - Age group 81–90
  - Diagnoses: Syncope, Dehydration, Chest Pain

---

## 🤖 Model Performance

| Model             | Accuracy | AUC  | Sensitivity | Specificity | MAE  |
|------------------|----------|------|-------------|-------------|------|
| Logistic Regression | 0.76     | 0.84 | 0.70        | 0.82        | 0.28 |
| **Random Forest**    | **0.82** | 0.76 | **0.88**     | 0.82        | **0.18** |
| Decision Tree     | 0.77     | 0.73 | 0.82        | 0.78        | 0.23 |

> 🏆 **Best Model**: Random Forest — highest accuracy and sensitivity.

---

## ✅ Recommendations
- Integrate predictive model into triage workflow for real-time decision support.
- Update triage protocols to flag:
  - Older patients (especially 81+)
  - Cases with "elevated" blood pressure
  - Diagnoses with high flip likelihood
- Conduct regular audits and model retraining to maintain predictive accuracy.

---

## 💡 Tools & Technologies
- Python (Pandas, Scikit-learn)
- Jupyter Notebook
- Descriptive Statistics
- Machine Learning Models (LogReg, RF, DT)
- Matplotlib/Seaborn for visualizations

---

## 📎 Next Steps
- Deploy model via a user interface (streamlit or Power BI integration).
- Collaborate with clinical teams to validate triage adjustments.
- Monitor patient outcomes and flip rates post-implementation.

---

## 👩‍💻 Author
**Kavya Chandran**  
[LinkedIn](https://www.linkedin.com/in/kavyac15/) | [GitHub](https://github.com/Kavya150493)

---

## 📜 License
This project is for educational and demonstration purposes only.

