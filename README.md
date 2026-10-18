# CSET485 – AI and Society | Assignment 1

## German Credit Data: Model Comparison, Bias and Fairness Analysis

### 📌 Project Overview
This project analyzes the German Credit Data dataset to understand how machine learning models make credit-risk predictions and how their decisions can be affected by model selection, omitted variables, subgroup differences, and fairness considerations.

The assignment compares Linear Regression and Logistic Regression, investigates possible Simpson’s Paradox and omitted variable bias, examines high-confidence prediction errors, and evaluates fairness across age groups.

### 🎯 Objectives
- Compare Linear Regression and Logistic Regression for binary credit-risk classification.
- Investigate possible subgroup differences and Simpson’s Paradox.
- Analyze coefficient changes caused by omitting a variable.
- Examine high-confidence incorrect predictions.
- Evaluate fairness metrics across age groups at different classification thresholds.
- Understand the social and ethical implications of AI-based credit decisions.

### 📊 Dataset
**Dataset:** German Credit Data  
**Source:** [UCI Machine Learning Repository – Statlog (German Credit Data)](https://archive.ics.uci.edu/dataset/144/statelog%2Bgerman%2Bcredit)

- 1,000 instances
- 20 input features
- Binary credit-risk target
- Train-test split: 70% training and 30% testing
- Random seed: `133`

The target variable is mapped to `1` for good credit risk (approval) and `0` for bad credit risk (rejection).

### 🛠️ Technologies Used
- Python
- Jupyter Notebook
- Pandas and NumPy
- Scikit-learn
- Statsmodels
- Matplotlib and Seaborn

### ⚙️ Methodology
1. **Data Preprocessing:** Load the dataset, inspect data quality, encode categorical features, and scale numerical features where required.
2. **Model Comparison:** Train Linear Regression and Logistic Regression and compare their classification decisions.
3. **Simpson’s Paradox Investigation:** Compare selected relationships across age-based subgroups.
4. **Omitted Variable Bias:** Examine coefficient changes after removing age from the regression model.
5. **Adversarial Error Analysis:** Identify high-confidence incorrect predictions and explore patterns in those cases.
6. **Fairness Evaluation:** Compare fairness metrics across age groups at different classification thresholds.
7. **Ethical Reflection:** Discuss model limitations, potential bias, and the implications of automated credit decisions.

### 🚀 How to Run
1. Clone or download this repository.
2. Install the required Python libraries:

   ```bash
   pip install pandas numpy scikit-learn statsmodels matplotlib seaborn jupyter
   ```

3. Download the German Credit Data file from the UCI source linked above.
4. Place `german.data` in the location expected by the notebook, or update the dataset path in the notebook.
5. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open the assignment notebook and run all cells from top to bottom.

### 📁 Repository Structure

```text
CSET485-AI-Society-Assignment1/
├── CSET485_Assignment1_German_Credit.ipynb
├── README.md
└── german.data   # Dataset, if included
```

The actual notebook and dataset filenames may differ depending on the files included in this repository.

### ⚠️ Limitations
The analysis uses a relatively small dataset and selected statistical models. Observed coefficient changes or subgroup differences do not automatically establish causal relationships. Fairness results also depend on the chosen metric, age-group definition, and classification threshold.

### 👨‍🎓 Course Information
- **Course:** CSET485 – AI and Society
- **Assignment:** Assignment 1
- **Student:** Vasu Aggarwal
- **Roll Number:** 0133

### 📚 References
- [UCI Machine Learning Repository – Statlog (German Credit Data)](https://archive.ics.uci.edu/dataset/144/statelog%2Bgerman%2Bcredit)
- Assignment instructions and course materials.

---

*This repository contains the notebook and analysis prepared for academic purposes as part of the AI and Society course.*
