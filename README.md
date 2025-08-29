# HR Attrition Analysis: Insights and Predictive Modelling  

## 📌 Project Overview  
This project explores employee attrition using the IBM HR dataset.  
The aim is to understand workforce turnover, identify the factors driving attrition,  
and build predictive models to help organisations design effective retention strategies.  

---

## 🎯 Objectives  
1. **Understand Current Turnover Rates**  
   - Measure the overall employee attrition rate.  
   - Analyse demographic distributions of attrition by age, gender, education, department, and job role.  

2. **Identify Key Factors Influencing Turnover**  
   - Explore job satisfaction and work–life balance (JobSatisfaction, JobInvolvement, WorkLifeBalance, EnvironmentSatisfaction).  
   - Assess salary-related factors (MonthlyIncome, PercentSalaryHike).  
   - Evaluate benefits and other drivers (StockOptionLevel, OverTime, BusinessTravel, DistanceFromHome).  

3. **Build Predictive Models**  
   - Use Logistic Regression and Random Forest to predict employee attrition.  
   - Handle class imbalance with SMOTE.  
   - Evaluate models with Accuracy, Precision, Recall, F1-Score, ROC-AUC, and PR-AUC.  

---

## 📊 Dataset  
- **Source:** IBM HR Analytics dataset (synthetic).  
- **Records:** 1,470 employees  
- **Features:** 35 demographic, job-related, and compensation attributes  
- **Target:** `Attrition` (Yes/No)  
- **Class Distribution:** ~16% Yes, ~84% No  
- **Missing Values:** None  

### Key Columns  
- **Age, Gender, Department, JobRole** → demographic attributes  
- **MonthlyIncome, PercentSalaryHike, StockOptionLevel** → compensation factors  
- **JobSatisfaction, WorkLifeBalance, JobInvolvement, EnvironmentSatisfaction** → satisfaction/engagement measures  
- **OverTime, BusinessTravel, DistanceFromHome** → work-related drivers  

---

## 🔍 Project Steps  
1. **Data Overview** – structure, descriptive statistics, class balance  
2. **Exploratory Data Analysis (EDA)** – turnover by demographics and key factors  
3. **Pre-processing** – encoding, scaling, handling imbalance with SMOTE  
4. **Modelling** – Logistic Regression and Random Forest with Stratified CV  
5. **Evaluation** – classification reports, confusion matrices, ROC/PR curves, feature importances  
6. **Insights & Recommendations** – actionable strategies for HR  

---

## 💡 Key Insights  
- Overall attrition rate is **~16%**.  
- **Younger, single employees** and those in **Sales roles** show higher turnover.  
- **OverTime** is the strongest driver of attrition.  
- Poor **work–life balance** and low **job satisfaction** significantly increase attrition risk.  
- Employees with **lower income** and **smaller salary hikes** are more likely to leave.  
- Random Forest achieved the best predictive performance (**ROC-AUC ≈ 0.82**).  

---

## 🏆 Conclusion  
This analysis shows that attrition is influenced by **workload, satisfaction, and compensation factors**.  
Predictive models can identify at-risk employees with strong accuracy,  
helping organisations design **targeted retention strategies** such as:  
- Reducing overtime  
- Enhancing work–life balance  
- Improving compensation structures  
- Focusing retention programmes on high-risk groups (younger employees, Sales department)  

---

## 🚀 How to Run  
You can run the notebook directly in **Google Colab** (no setup required):  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/amitkumarbhade/HR_Attrition_Analysis/blob/main/HR_Attrition_Analysis.ipynb)  

Steps:  
1. Upload the notebook (`HR_Attrition_Analysis.ipynb`) to your Colab/drive.  
2. Upload the dataset file (`HR Data.csv`) when prompted.  
3. Run cells sequentially to reproduce analysis and results.  

---

