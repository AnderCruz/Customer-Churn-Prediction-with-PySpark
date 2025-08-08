# 🔁 Customer Churn Prediction with PySpark

*A classification model using Spark DataFrames and MLlib*

This project aims to support the **marketing team** in predicting whether a customer is likely to **cancel a service (churn)**. With a reliable classification model, the company can take proactive measures to **retain customers** and reduce churn rates.

📊 Developed by **Nowa Analytics**, a data consulting firm specializing in Big Data, machine learning, and data-driven decision-making.

---

## 🎯 Problem Statement

The marketing department has noticed a growing **customer churn problem** and needs a tool to help **predict which customers are at risk** of cancelling their services.

To address this, we developed a **machine learning classification model** that predicts customer churn based on key features, such as:

* Contract duration
* Service type
* Tenure
* Subscription level
* Payment method
* and more

---

## ⚙️ Solution Approach

We use **PySpark** and **Spark MLlib** to implement a complete **Machine Learning Pipeline**, including:

* ✅ Data preparation with **Spark SQL**
* ✅ Feature engineering with **DataFrame APIs**
* ✅ Model training with **classification algorithms**
* ✅ **Hyperparameter tuning** using `CrossValidator` and `ParamGridBuilder`
* ✅ Model evaluation and validation
* ✅ Delivering a final optimized model ready to classify new customers

---

## 🧪 Techniques Used

* **Data Processing**:

  * Handling null values
  * Encoding categorical features (`StringIndexer`, `OneHotEncoder`)
  * Feature assembly (`VectorAssembler`)
* **Modeling**:

  * Logistic Regression
  * Decision Tree Classifier
  * Random Forest Classifier
* **Model Optimization**:

  * Cross-validation
  * Hyperparameter tuning
* **Model Evaluation**:

  * Accuracy
  * Precision, Recall, F1-score
  * Confusion Matrix
  * ROC-AUC (when applicable)

---

## 📁 Project Structure

```
📦 churn-prediction-spark
│
├── data/                  # Input dataset (CSV or Parquet)
├── notebooks/             # Jupyter Notebooks with step-by-step pipeline
├── src/                   # Python scripts for preprocessing and modeling
│   ├── data_cleaning.py
│   ├── churn_pipeline.py
│   └── model_evaluation.py
├── results/               # Evaluation metrics, logs, and model artifacts
├── README.md              # Project documentation
└── requirements.txt       # Required Python libraries
```

---

## 📊 Dataset Description

The dataset was provided by the marketing team and includes customer-level data such as:

* `customer_id`
* `contract_type`
* `tenure` (in months)
* `internet_service`
* `monthly_charges`
* `total_charges`
* `payment_method`
* `churn` (target: yes/no)

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/churn-prediction-spark.git
cd churn-prediction-spark
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Start a PySpark session and run the notebook in `notebooks/` or execute the scripts in `src/`.

4. To run the full training pipeline via Spark:

```bash
spark-submit src/churn_pipeline.py
```

---

## ✅ Results

After tuning and validating multiple models, the **Random Forest Classifier** achieved the best performance:

| Metric   | Value |
| -------- | ----- |
| Accuracy | 0.87  |
| F1-Score | 0.84  |
| ROC AUC  | 0.91  |

> The model is now ready to be deployed to classify **new customers** as likely or unlikely to churn.

---

## 🧠 Key Insights

* Contract type and tenure are among the most significant predictors of churn.
* Prepaid customers with short tenures are more likely to churn.
* Hyperparameter tuning had a significant impact on model performance.

---

## 🏢 About Nowa Analytics

**Nowa Analytics** is a boutique data consultancy specializing in advanced analytics, machine learning, and data engineering. We help organizations unlock value from their data and make better strategic decisions.

📍 Offices in São Paulo, Madrid, and London
🌐 [nowaanalytics.com](http://nowaanalytics.com) *(replace with actual site)*

---

## 📬 Contact

* 📧 [contact@nowaanalytics.com](mailto:contact@nowaanalytics.com)
* 💼 [LinkedIn – Nowa Analytics](https://linkedin.com/company/nowaanalytics)
