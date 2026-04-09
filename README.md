# End to End Data Science Project

### Workflows--ML Pipeline

1. Data Ingestion
2. Data Validation
3. Data Transformation-- Feature Engineering,Data Preprocessing
4. Model Trainer
5. Model Evaluation- MLFLOW,Dagshub

## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py



# 🚀 End-to-End MLOps Pipeline with Flask Deployment

A production-ready Machine Learning system built using a modular architecture with complete MLOps practices including data ingestion, validation, transformation, model training, evaluation, MLflow tracking, model registry (DagsHub), and a Flask-based web application for real-time predictions.

---

## 📌 Project Overview

This project demonstrates how to build a **scalable, maintainable, and production-style ML pipeline** from scratch.

It follows a **config-driven modular architecture** and integrates **MLflow + DagsHub** for experiment tracking and model versioning.

---

## 🧠 Key Features

✔️ Modular ML pipeline (clean architecture)
✔️ Config-driven system (no hardcoding)
✔️ Data ingestion, validation, transformation
✔️ Model training using ElasticNet
✔️ Model evaluation with metrics (RMSE, MAE, R²)
✔️ MLflow experiment tracking
✔️ Model registry with versioning (DagsHub)
✔️ Flask web app for real-time prediction
✔️ End-to-end automation via pipeline

---

## 🏗️ Project Architecture

```
src/
 ├── components/
 ├── pipeline/
 ├── config/
 ├── entity/
 ├── utils/
 ├── constants/
```

---

## 🔄 Pipeline Flow

```
Data Ingestion
   ↓
Data Validation
   ↓
Data Transformation
   ↓
Model Training
   ↓
Model Evaluation
   ↓
MLflow Tracking + Model Registry
```

---

## 📦 Artifacts Generated

```
artifacts/
 ├── data_ingestion/
 ├── data_validation/
 ├── data_transformation/
 │    ├── train.csv
 │    └── test.csv
 ├── model_trainer/
 │    └── model.joblib
 ├── model_evaluation/
 │    └── metric.json
```

---

## 📊 Model Details

* Algorithm: **ElasticNet Regression**
* Hyperparameters: Managed via `params.yaml`
* Evaluation Metrics:

  * RMSE
  * MAE
  * R² Score

---

## 🔥 MLflow + DagsHub Integration

* Tracks:

  * Parameters
  * Metrics
  * Model artifacts
* Supports:

  * Experiment comparison
  * Model versioning
* Model registered in **DagsHub MLflow Registry**

---

## 🌐 Flask Web Application

### Routes

* `/` → Input form UI
* `/train` → Run full pipeline
* `/predict` → Get predictions

### Flow

```
User Input → Flask App → Prediction Pipeline → Model → Output
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone <your-repo-url>
cd <repo-folder>
```

---

### 2️⃣ Create Virtual Environment

```bash
conda create -p venv python=3.10 -y
conda activate venv
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Set Environment Variables (DagsHub MLflow)

```bash
set MLFLOW_TRACKING_URI=https://dagshub.com/<username>/<repo>.mlflow
set MLFLOW_TRACKING_USERNAME=<your-username>
set MLFLOW_TRACKING_PASSWORD=<your-token>
```

---

### 5️⃣ Run Full Pipeline

```bash
python main.py
```

---

### 6️⃣ Run Flask App

```bash
python app.py
```

Open browser:

```
http://localhost:8080
```

---

## 🧠 Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* MLflow
* DagsHub
* Flask
* Joblib

---

## 💣 Highlights

* Built **end-to-end ML system from scratch**
* Implemented **real-world MLOps practices**
* Integrated **experiment tracking + model registry**
* Developed **deployable web application**

---

## 📄 Resume Highlight

> Built a production-ready end-to-end ML pipeline with modular architecture, MLflow experiment tracking, model versioning using DagsHub, and a Flask-based web application for real-time predictions.

---

## 🚀 Future Improvements

* Docker containerization
* CI/CD pipeline (GitHub Actions)
* FastAPI deployment
* Model monitoring

---

## 🤝 Connect

If you found this project useful, feel free to ⭐ the repo and connect!

---

## 🔥 Final Thought

> “This is not just a model — it’s a complete ML system.”
