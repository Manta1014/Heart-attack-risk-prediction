# 🫀 Heart Attack Risk Prediction

This project investigates how lifestyle variables affect the risk of heart attack in individuals who **do not have a family history** of heart disease. Using R, we performed exploratory data analysis, logistic regression modeling, and hypothesis testing.

---

## 📌 Research Question

> **Is there a relationship between exercise hours, sleep hours, and stress level and the risk of heart attack in people with no family history of heart attacks?**

---

## 🧪 Dataset Overview

- **Source**: Simulated health dataset with lifestyle and medical variables
- **Target Variable**: `heart_attack_risk` (binary: 0 = no risk, 1 = risk)
- **Filtered Group**: Individuals with `family_history == 0`

### ✳️ Key Variables Used
| Type          | Variable              |
|---------------|------------------------|
| Explanatory   | `exercise_hrs_week`    |
|               | `sleep_hrs`            |
|               | `stress_level`         |
| Response      | `heart_attack_risk`    |

---

## 📊 Analytical Methods

### 1. **Data Tidying**
- Selected relevant variables and cleaned column names
- Separated dataset based on family history

### 2. **Exploratory Data Analysis**
- Compared distributions of stress, sleep, and exercise levels
- Used PMFs and boxplots to visualize differences by heart attack risk group

### 3. **Modeling**
- Trained 5 logistic regression models using combinations of predictors
- Evaluated accuracy using training accuracy and cross-validation error

### 4. **Hypothesis Testing**
- Tested for significant differences in proportions of heart attack risk between:
  - High vs Low Stress
  - High vs Low Sleep
  - High vs Low Exercise
- All p-values > 0.05 → Failed to reject the null hypothesis

---

## 📈 Results Summary

- **Model 1** (Exercise hours only) had the best accuracy (~61.7%) and lowest CV error
- No lifestyle factor alone showed a statistically significant impact on heart attack risk
- Large class imbalance (many more with no risk) affected detection power

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Final_project.Rmd` | R Markdown file with full analysis |
| `heart_attack_df.xls` | Raw dataset |
| `Final_project.pdf` | Final report (formatted) |
| `Heart_Attack_presentation_CDS101_2024.pptx` | Project presentation slides |
| `README.md` | This file |

---

## 🧠 Team Members
- Wonjune Lee (Manta1014)
- Giselle Rahimi, Jiwon Jung, Pilar Golar, Jiseon Kim, Sukyoung Yoon, Yoonhye Cho

---

## 🛠 Technologies Used

- **Language**: R  
- **Packages**: `tidyverse`, `infer`, `modelr`, `boot`  
- **Environment**: RStudio, GitHub

---

## 📬 Contact

If you have any questions or suggestions about this project, feel free to reach out via [GitHub](https://github.com/Manta1014).

---
