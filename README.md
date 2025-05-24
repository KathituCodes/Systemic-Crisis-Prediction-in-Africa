# Systemic, Banking, and Inflation Crises in Africa – ML Modeling

This project explores the **"Systemic Crisis, Banking Crisis, Inflation Crisis in Africa"** dataset sourced from Kaggle. The primary objective is to build a **Machine Learning classification model** to **predict the likelihood of a systemic financial crisis** using macroeconomic indicators such as inflation rates, among others. The objective is to identify which algorithm performs best in classifying crisis occurrences and handling class imbalance using SMOTE.

The dataset spans **13 African countries** from **1860 to 2014**, covering events related to:

* Banking Crises
* Debt Crises
* Financial Crises
* Inflation Crises
* Systemic Crises

## 🌍 Countries Included

* Algeria
* Angola
* Central African Republic
* Ivory Coast
* Egypt
* Kenya
* Mauritius
* Morocco
* Nigeria
* South Africa
* Tunisia
* Zambia
* Zimbabwe

---

## Project Steps

### 1. **Data Loading and Preprocessing**

* The dataset was loaded using `pandas`.
* Exploratory analysis was done to understand the structure and content of the data.
* Irrelevant or redundant features were removed, and necessary columns were selected.
* Null values were handled appropriately.
* Label encoding or one-hot encoding was used for categorical variables (where needed).
* Features and target variables were separated.

### 2. **Train-Test Split**

* The dataset was split into training and testing sets using `train_test_split()` from `sklearn.model_selection`.

### 3. **Model Building – Baseline Evaluation**

* Three classification algorithms were trained and evaluated:

  * **Decision Tree Classifier**
  * **Random Forest Classifier**
  * **K-Nearest Neighbors (KNN)**
* Each model’s accuracy and classification report were generated to compare performance.
* The aim was to determine the best-performing model before addressing the class imbalance.

### 4. **Class Imbalance Handling – SMOTE**

* **SMOTE (Synthetic Minority Over-sampling Technique)** was applied using `imblearn.over_sampling.SMOTE` to balance the target class distribution.
* After SMOTE, the data was re-split and the models were retrained.

### 5. **Model Evaluation After SMOTE**

* Each of the previously trained models was retrained on the balanced dataset.
* Evaluation metrics (Accuracy, Precision, Recall, F1-score) were used to assess improvements.
* Model performance was compared before and after SMOTE.

---

## ⚙️ Technologies Used

* Python
* Jupyter Notebook
* pandas, numpy
* scikit-learn
* imbalanced-learn (for SMOTE)
* matplotlib & seaborn (for visualization)

---

## 📊 Key Insights

* Class imbalance significantly impacted model performance.
* SMOTE improved classification metrics, especially for minority classes.
* Among the tested algorithms,  `Random Forest Model` performed best post-balancing.

\* *(Replace with the actual best model based on your final results.)*

---

## 📁 Files

* `Systemic_Crisis,_Banking_Crisis,_inflation_Crisis_In_Africa.ipynb` – Main analysis notebook

---

## 🚀 How to Run

1. Clone this repository
2. Install requirements:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
---

## 🤝 Collaboration & Discussion

I encourage all contributors to **discuss alternative strategies** to enhance model performance and gain deeper insights into financial crises in African economies.

Contributions, questions, and suggestions are welcome! Please open an issue or submit a pull request.

---



