# 🫀 Heart Disease Risk Assessment Agent using ML

An end-to-end Machine Learning pipeline and deployment application designed to predict the likelihood of heart disease in patients based on clinical health metrics.

---

## 📌 Project Architecture & Workflow

The pipeline takes clinical patient data through missing value handling, feature scaling, train-test splitting, and evaluation across multiple classifiers to find the optimal diagnostic model.

<Image src="image_agent_tag_17149486199877850227" alt="Framework of the Heart Disease Prediction System showing preprocessing, dataset splitting, training, and testing." caption="Heart Disease Risk Assessment System Workflow" />

---

## 🚀 Features

* **Data Preprocessing & Cleaning:** Handles missing values, deduplication, and standardizes continuous numerical attributes using `StandardScaler`.
* **Multi-Model Comparison:** Trains and benchmarks 6 standard machine learning algorithms:
  * Logistic Regression
  * Random Forest Classifier
  * XGBoost Classifier
  * Support Vector Machine (SVM)
  * K-Nearest Neighbors (KNN)
  * Multi-Layer Perceptron (MLP)
* **Comprehensive Metrics:** Evaluates models based on Accuracy, Precision, Recall, F1-Score, ROC-AUC, and Confusion Matrices.
* **Web Deployment Ready:** Easy deployment configuration for cloud platforms like **Render**.

---

## 📊 Dataset

This project utilizes the famous **Heart Disease Dataset** available on Kaggle.

* **Source:** [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
* **Key Features:** Age, Sex, Chest Pain Type (`cp`), Resting Blood Pressure (`trestbps`), Serum Cholesterol (`chol`), Fasting Blood Sugar (`fbs`), Resting ECG (`restecg`), Max Heart Rate (`thalach`), Exercise Induced Angina (`exang`), ST Depression (`oldpeak`), Slope, Major Vessels (`ca`), and Thalassemia (`thal`).
* **Target:** `1` (Presence of Heart Disease) | `0` (Absence of Heart Disease)

---

## 📂 Project Structure

```text
├── app.py                # Main web application entry point (Streamlit / FastAPI)
├── heart.csv             # Kaggle heart disease dataset
├── model_training.py     # Data preprocessing & ML pipeline script
├── requirements.txt      # Project dependencies for deployment
└── README.md             # Project documentation
