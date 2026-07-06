Youtube-Comment-Sentiment-Analysis
==============================

📌 Overview

This project is an end-to-end MLOps implementation for YouTube Comment Sentiment Analysis. It automates the complete machine learning lifecycle—from data ingestion and preprocessing to model training, experiment tracking, testing, deployment, and real-time sentiment prediction.

The project demonstrates production-ready MLOps practices using DVC, MLflow, GitHub Actions, Docker, Flask, and a Chrome Extension for analyzing YouTube comments directly from the browser.


🚀 Features
- End-to-End Machine Learning Pipeline
- Automated Data Versioning with DVC
- Text Preprocessing and TF-IDF Vectorization
- LightGBM Model Training
- Experiment Tracking using MLflow
- Model Registry Integration
- Automated Testing with Pytest
- CI/CD Pipeline using GitHub Actions
- Dockerized Application
- REST API using Flask
- Chrome Extension for Real-Time Sentiment Prediction
- Reproducible Machine Learning Workflow

🛠️ Tech Stack

| Category | Technologies |
|-----------|--------------|
| Language | Python |
| Machine Learning | Scikit-learn, LightGBM |
| NLP | TF-IDF Vectorizer |
| Experiment Tracking | MLflow |
| Data Versioning | DVC |
| CI/CD | GitHub Actions |
| API | Flask |
| Containerization | Docker |
| Testing | Pytest |
| Version Control | Git & GitHub |

📂 Project Structure

```text
Youtube-Comment-Sentiment-Analysis
│
├── .github/
│   └── workflows/
│       └── cicd.yml
│
├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
│
├── flask_app/
│
├── src/
│   ├── data_ingestion/
│   ├── data_preprocessing/
│   ├── model_building/
│   ├── model_evaluation/
│   ├── register_model/
│   └── utils/
│
├── tests/
│
├── dvc.yaml
├── dvc.lock
├── Dockerfile
├── requirements.txt
├── app.py
└── README.md
```


⚙️ MLOps Pipeline

```text
Data Collection
      │
      ▼
Data Validation
      │
      ▼
Data Preprocessing
      │
      ▼
Feature Engineering
      │
      ▼
Model Training
      │
      ▼
Model Evaluation
      │
      ▼
MLflow Experiment Tracking
      │
      ▼
Model Registration
      │
      ▼
Flask REST API
      │
      ▼
Chrome Extension
```

---


Machine Learning Workflow

1. Data Ingestion
2. Data Validation
3. Data Preprocessing
4. TF-IDF Feature Engineering
5. Train LightGBM Classifier
6. Evaluate Model Performance
7. Track Experiments with MLflow
8. Register Best Model
9. Deploy using Flask API
10. Predict Sentiment through Chrome Extension



🧪 Installation

### Clone the Repository

```bash
git clone https://github.com/sarthakag12/Youtube-Comment-Sentiment-Analysis.git

cd Youtube-Comment-Sentiment-Analysis
```

### Create Virtual Environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

▶️ Run the DVC Pipeline

```bash
dvc repro
```

---

## 📈 Start MLflow

```bash
mlflow ui
```

Open:

```
http://localhost:5000
```

---

## 🚀 Run the Flask API

```bash
python app.py
```

---

## 🧪 Run Unit Tests

```bash
pytest
```

---

## 🐳 Docker

### Build Docker Image

```bash
docker build -t youtube-comment-sentiment .
```

### Run Docker Container

```bash
docker run -p 5000:5000 youtube-comment-sentiment
```

---

## 📡 REST API

### POST `/predict`

### Request

```json
{
    "comment": "This video is amazing!"
}
```

### Response

```json
{
    "prediction": "Positive"
}
```

---

## 🌐 Chrome Extension

The Chrome Extension allows users to analyze YouTube comments directly from their browser.

### Features

- Fetch YouTube comments
- Send comments to Flask API
- Display sentiment prediction
- Real-time inference using the trained ML model

---


