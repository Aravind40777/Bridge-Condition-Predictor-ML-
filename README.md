Bridge Condition Predictor using Machine Learning

Project Overview

The **Bridge Condition Predictor** is an end-to-end Machine Learning application that predicts whether a bridge is in a **Good/Safe** or **Poor/Unsafe** condition based on structural and operational characteristics.

The project follows the complete Machine Learning lifecycle, including:

- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Engineering
- Model Training
- Hyperparameter Tuning
- Model Evaluation
- Streamlit Web Application
- Cloud Deployment

---

## 🌐 Live Demo

🔗 **Application:**  
https://9zautjk6lwwv4rjvj8g95t.streamlit.app/

---

## 🚀 Features

- 🌉 Predicts bridge condition instantly
- 📊 Probability score for each prediction
- 🤖 Tuned Random Forest Machine Learning model
- 📈 Real-time prediction monitoring
- 📝 Prediction history logging
- 🎨 Interactive Streamlit user interface
- ☁️ Deployed on Streamlit Community Cloud

---

# 📂 Project Structure

```
Bridge-Condition-Predictor-ML-
│
├── app.py
├── requirements.txt
├── runtime.txt
│
├── data/
│   └── bridge_data.csv
│
├── models/
│   ├── final_bridge_model.pkl
│   ├── final_bridge_scaler.pkl
│   └── final_bridge_features.pkl
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── predict.py
│
├── notebooks/
│   ├── Sprint-1_EDA.ipynb
│   ├── Sprint-2_Modeling.ipynb
│   └── Sprint-3_Optimization.ipynb
│
└── logs/
    ├── predictions.log
    └── metrics.json
```

---

# ⚙️ Machine Learning Workflow

### 1️⃣ Data Collection

Bridge inspection dataset containing:

- Age of Bridge
- Traffic Volume
- Material Type
- Maintenance Level
- Bridge Condition

---

### 2️⃣ Exploratory Data Analysis (EDA)

Performed:

- Missing value analysis
- Class distribution
- Correlation analysis
- Distribution plots
- Outlier detection
- Feature importance exploration

---

### 3️⃣ Data Preprocessing

- Label Encoding
- One-Hot Encoding
- Feature Scaling (StandardScaler)
- Train-Test Split

---

### 4️⃣ Feature Engineering

Created additional domain-specific features including:

- Traffic per Year
- Age Squared
- Age Bucket
- High Stress Indicator
- Concrete Age Interaction
- Steel Traffic Interaction
- Neglect Score

---

### 5️⃣ Model Training

The following machine learning algorithms were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- Naive Bayes
- Gradient Boosting

---

# 📊 Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score | Remarks |
|------|---------:|----------:|-------:|---------:|---------|
| Logistic Regression | 82.35% | 46.67% | 35.00% | 40.00% | Good Generalization |
| Decision Tree | 84.87% | 54.17% | 65.00% | 59.09% | Overfitting Observed |
| Random Forest | **89.92%** | **70.00%** | **70.00%** | **70.00%** | Best Baseline Model |
| Support Vector Machine | 85.71% | 63.64% | 35.00% | 45.16% | Good Generalization |
| Naive Bayes | 84.03% | 53.33% | 40.00% | 45.71% | Good Generalization |
| Gradient Boosting | 86.55% | 58.33% | 70.00% | 63.64% | Slight Overfitting |

---

# 🏆 Final Model

The final deployed model is a **Random Forest Classifier** optimized using:

- RandomizedSearchCV
- GridSearchCV

### Model Pipeline

- Feature Engineering
- StandardScaler
- Random Forest Classifier
- Joblib Model Serialization

---

# 📈 Key Observations

- ✅ Random Forest outperformed all baseline models.
- ✅ High Recall for **Poor/Unsafe** bridges is prioritized because missing a deteriorating bridge is a critical safety risk.
- ✅ Hyperparameter tuning improved model generalization.
- ✅ Cross-validation confirmed stable model performance.

---

# ⭐ Important Features

The most influential features are:

- Age of Bridge
- Traffic per Year
- Neglect Score
- Traffic Volume
- Maintenance Level

---

# 🎯 Prediction Classes

| Class | Meaning |
|--------|---------|
| ✅ 0 | Good / Safe Bridge |
| ⚠️ 1 | Poor / Unsafe Bridge |

---

# 🛠 Tech Stack

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Scikit-learn
- Joblib
- Streamlit
- Matplotlib
- Seaborn

### Tools

- Jupyter Notebook
- Git
- GitHub
- Streamlit Community Cloud

---

# 💻 Installation

## Clone Repository

```bash
git clone https://github.com/Aravind40777/Bridge-Condition-Predictor-ML-.git
```

---

## Navigate to Project

```bash
cd Bridge-Condition-Predictor-ML-
```

---

## Create Virtual Environment

```bash
python -m venv myenv
```

---

## Activate Virtual Environment

### Windows

```bash
myenv\Scripts\activate
```

### Linux / macOS

```bash
source myenv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run the Application

```bash
streamlit run app.py
```

---

# 📸 Application Screenshots

<img width="1913" height="956" alt="Screenshot 2026-07-01 235816" src="https://github.com/user-attachments/assets/0d12c556-da1e-4262-b7e4-e1ede3acaadd" />




---

## Prediction Result
<img width="1913" height="956" alt="Screenshot 2026-07-01 235816" src="https://github.com/user-attachments/assets/69084103-5945-4e5c-bd9e-31b5988fcb99" />




---

# ☁️ Deployment

The application is deployed using **Streamlit Community Cloud**.

Live Application:

https://9zautjk6lwwv4rjvj8g95t.streamlit.app/

---


GitHub

https://github.com/Aravind40777

LinkedIn

https://www.linkedin.com/in/aravindbhukya06/

---

# ⭐ If you found this project useful

Please consider giving it a ⭐ on GitHub!

