# 🏥 Health Insurance Cost Predictor

A Machine Learning-powered web application that predicts an individual's health insurance premium based on demographic, lifestyle, and medical information.

Built using **Python**, **Scikit-Learn**, and **Streamlit**, this project demonstrates the complete machine learning workflow from data preprocessing and feature engineering to model deployment.

---

## 🚀 Live Demo

Add your deployed Streamlit URL here:

```text
https://your-app-url.streamlit.app
```

---

## 📌 Problem Statement

Health insurance premiums depend on multiple factors such as:

* Age
* Income
* BMI
* Smoking habits
* Medical history
* Genetic risk
* Insurance plan selection

The objective of this project is to accurately estimate insurance costs using machine learning models and provide an easy-to-use web interface for users.

---

## ✨ Features

* Interactive Streamlit web application
* Real-time premium prediction
* Medical history risk assessment
* Automated feature engineering
* Data preprocessing pipeline
* Separate models for different age groups
* Input validation through user-friendly forms

---

## 🛠️ Tech Stack

### Programming Language

* Python

### Machine Learning

* Scikit-Learn
* Joblib

### Data Processing

* Pandas
* NumPy

### Deployment

* Streamlit

---

## 📊 Input Features

| Feature              | Description                              |
| -------------------- | ---------------------------------------- |
| Age                  | User age                                 |
| Number of Dependants | Family dependants                        |
| Income in Lakhs      | Annual income                            |
| Genetic Risk         | Risk score from family history           |
| Gender               | Male/Female                              |
| Marital Status       | Married/Unmarried                        |
| BMI Category         | Normal, Overweight, Obesity, Underweight |
| Smoking Status       | Non-Smoker, Occasional, Regular          |
| Employment Status    | Salaried, Self-Employed, Freelancer      |
| Region               | Geographic region                        |
| Medical History      | Existing medical conditions              |
| Insurance Plan       | Bronze, Silver, Gold                     |

---

## 🧠 Feature Engineering

The application performs custom feature engineering before making predictions.

### Medical Risk Score

Medical conditions are mapped to risk scores:

| Condition           | Risk Score |
| ------------------- | ---------- |
| Heart Disease       | 8          |
| Diabetes            | 6          |
| High Blood Pressure | 6          |
| Thyroid             | 5          |
| No Disease          | 0          |

The total risk score is normalized to create a **Normalized Risk Score** feature used by the machine learning model.

---

## 🤖 Machine Learning Approach

The project uses two separate trained models:

### Young Customer Model

Used for users aged **25 years or below**.

### General Customer Model

Used for users aged **above 25 years**.

This segmentation allows the system to better capture age-specific premium patterns and improve prediction accuracy.

---

## 📂 Project Structure

```text
health-insurance-predictor/
│
├── main.py
├── prediction_helper.py
│
├── artifacts/
│   ├── model_young.joblib
│   ├── model_rest.joblib
│   ├── scaler_young.joblib
│   └── scaler_rest.joblib
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/health-insurance-predictor.git

cd health-insurance-predictor
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Mac/Linux:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run Locally

```bash
streamlit run main.py
```

Open:

```text
http://localhost:8501
```

---

## 📈 Sample Workflow

1. Enter personal information.
2. Select insurance plan.
3. Choose medical history and lifestyle details.
4. Click **Predict**.
5. View estimated health insurance premium instantly.

---

## 🔮 Future Improvements

* Model explainability using SHAP
* Premium comparison across plans
* User authentication
* Database integration
* Cloud deployment with CI/CD
* Premium trend visualizations

---

## 📚 Learning Outcomes

Through this project I gained experience in:

* Data preprocessing
* Feature engineering
* Model training and evaluation
* Serialization using Joblib
* Streamlit application development
* End-to-end ML deployment
* Production-ready project structuring

---

## 👨‍💻 Author

**Mukul Chandravanshi**

LinkedIn: https://linkedin.com/in/your-profile

GitHub: https://github.com/your-github

---

## ⭐ Support

If you found this project useful, consider giving it a star on GitHub.

