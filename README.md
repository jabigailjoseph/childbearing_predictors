## **The Likelihood of Childbearing Based on Educational, Socioeconomic, and Interpersonal Factors**



### 📌 **Project Overview**

According to the **White House** (2023), the **CDC** reported that the U.S. birth rate has fallen to its lowest level in history[^1]. Researchers attribute this decades-long decline to several key factors:

- **Social and economic disparities**  
- **Increased age at parenthood**  
- **Changing societal norms**  

This project explores how **educational, socioeconomic, and interpersonal factors** impact the likelihood of individuals in the U.S. having children. By identifying the most impactful predictors, we aim to provide actionable insights for policymakers to better support Americans' decisions regarding childbearing.

---

### 🎯 **Project Objective**

The primary goal of this project is to **examine the relationship between five key factors and the likelihood of childbearing** using a **logistic regression model**.

The five factors analyzed are:  
1. 🏠 **Marital Status**  
2. 🎓 **Educational Attainment**  
3. 💼 **Income Level**  
4. 🏥 **Health Coverage**  
5. 🧑‍🤝‍🧑 **Sexual Orientation**  

The analysis identifies which of these factors **most significantly increase or decrease** the odds of individuals having children.

---

### 🧪 **Methodology**

- **Dataset**: Publicly available **National Survey of Family Growth (NSFG)** data  
- **Techniques**:  
   - Logistic Regression  
   - Confounding Assessment  
   - Multicollinearity Checks (VIF)  
   - AIC Analysis (Model Improvement)  
- **Tools**:  
   - **R Programming Language**  
   - Packages: `glm`, `pROC`, `car`, `ggplot2`  

---

### 📊 **Results**

#### **Key Findings**:  

- **Marital Status**: Individuals classified as *"Other"* (e.g., divorced, separated) have significantly lower odds (~4%) of having children compared to those who are *Married/Cohabiting*.  
- **Income Level**: Individuals with *Low Income* have odds reduced to ~42.6% compared to those with *High Income*.  
- **Education Level**: The presence of a college degree showed a modest reduction in odds, though it was not statistically significant (p > 0.05).  

#### **Performance Comparison**:  

| Metric                        | Baseline Model | Full Model |
|-------------------------------|----------------|------------|
| **Accuracy**                  | 66.9%          | 80.7%      |
| **AUC (Area Under the Curve)**| -              | 0.857      |

The full logistic regression model outperformed the baseline model significantly, as evidenced by higher accuracy and an **AUC score of 0.857**.

---

### 📈 **Visuals**

#### **ROC Curve for Full Model**  
![ROC Curve](./path_to_roc_image.png)  

#### **Odds Ratios Summary Table**  

| Variable          | Odds Ratio | CI Lower | CI Upper |
|-------------------|------------|----------|----------|
| **Marital Status** (Other) | 0.0408     | 0.0304   | 0.0538   |
| **Income** (Low Income)    | 0.4260     | 0.3192   | 0.5668   |
| **Education** (No Degree)  | 0.8036     | 0.6290   | 1.0242   |
| **Health Coverage**        | 0.7692     | 0.5795   | 1.0199   |
| **Sexual Orientation**     | 0.3724     | 0.1411   | 0.8636   |

---

### 📄 **Significance**

The results from this study will help:  

- Identify **key predictors** influencing childbearing decisions.  
- Inform policymakers on which **socioeconomic and interpersonal factors** require more support.  
- Enable **future research** on strategies to address declining fertility rates in the U.S.

---

### 🗂 **References**  

[^1]: White House, *Issue Brief on U.S. Fertility Rates*, 2023.  
[^2]: CDC, *National Survey of Family Growth (NSFG)*.  

---

This version is clean, organized, and takes full advantage of markdown formatting. Use the placeholder `path_to_roc_image.png` for your image path, and replace the reference links or footnotes where necessary. It will look professional on GitHub!

