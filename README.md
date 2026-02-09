# health-risk-prediction


# 🩺 Diabetes Risk Prediction — Decision Tree Classifier

## 📌 Project Overview

This project predicts whether an individual is likely to have diabetes based on demographic, lifestyle, and medical factors using a **Decision Tree Classifier**.

The goal is to demonstrate how **interpretable machine learning models** can be applied to healthcare-related problems while maintaining clarity and transparency.

**Sustainable Development Goal (SDG):**
**SDG 3 – Good Health and Well-being**

---

## 🎯 Problem Statement

Diabetes is a major public health challenge. Early identification of individuals at risk can support preventive care and better health outcomes.

This project answers the question:

> *Can we predict diabetes risk using simple, explainable decision rules derived from health data?*

---

## 📊 Dataset

* **Type:** Health and lifestyle dataset
* **Target Variable:**

  * `Diagnosis`

    * `Yes` → Diabetes
    * `No` → No Diabetes
* **Features Include:**

  * Age
  * BMI
  * Fasting Blood Sugar (FBS)
  * HbA1c
  * Gender
  * Family history of diabetes
  * Smoking status
  * Diet
  * Exercise
  * Blood pressure

The dataset was found to be **clean**, with no missing or duplicate values.

---

## ⚙️ Project Workflow

1. **Data Inspection**

   * Dataset overview and quality checks
2. **Preprocessing**

   * One-Hot Encoding for categorical features
   * Numerical features passed through directly
3. **Train–Test Split**

   * 80% training, 20% testing
4. **Model Training**

   * Decision Tree Classifier inside a pipeline
5. **Evaluation**

   * Accuracy, precision, recall, F1-score
6. **Visualization**

   * Decision tree plotted for interpretability
7. **Interpretation**

   * Clear explanation of decision rules in simple language
8. **Outputs**

   * Predictions and visualizations saved for reproducibility

---

## 📈 Model Performance

### Test Set

* **Accuracy:** ~92%
* Strong performance on unseen data
* **100% recall for diabetic cases**, meaning no positive cases were missed

### Training Set

* **Accuracy:** 100%

This indicates **mild overfitting**, which is common with decision trees.
Despite this, the model generalizes well and remains reliable for interpretation.

---

## 🌳 Decision Tree Insights (Summary)

* **Diet** is the most influential factor
* **Family history of diabetes** strongly increases risk
* **Age** and **blood sugar levels** further refine predictions
* The model’s logic aligns well with real-world medical understanding

---

## 📁 Repository Structure

```
health-risk-prediction/
│
├── data/
│   └── Diabetes_Classification.csv
│
├── notebooks/
│   └── diabetes_decision_tree.ipynb
│
├── Outputs/
│   ├── diabetes_decision_tree.png
│   └── prediction_results.csv
│
├── requirements.txt
└── README.md
```

---

## ▶️ How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/MarvellousAdedokun/health-risk-prediction
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open and run the notebook:

```
notebooks/diabetes_decision_tree.ipynb
```

---

## 🚧 Limitations

* Dataset size is relatively small
* Decision Trees can overfit without pruning
* Results are for educational purposes and not for clinical diagnosis

---

## 🔮 Future Improvements

* Apply pruning or depth control to reduce overfitting
* Compare performance with Random Forest or Gradient Boosting
* Expand dataset for better real-world coverage

---

## 🧠 Key Takeaway

This project shows how **interpretable machine learning** can be applied to healthcare problems, balancing performance with transparency and real-world relevance.

---

