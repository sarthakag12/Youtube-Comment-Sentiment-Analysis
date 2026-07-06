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


📊 Model Workflow
- Load Dataset
- Clean and preprocess comments
- Convert text into TF-IDF vectors
- Train LightGBM classifier
- Evaluate model performance
- Log experiments using MLflow
- Register the best-performing model
- Serve predictions through Flask API
- Consume predictions via Chrome Extension


🧪 Running the Project
1. Clone the Repository
git clone https://github.com/sarthakag12/Youtube-Comment-Sentiment-Analysis.git
cd Youtube-Comment-Sentiment-Analysis

2. Create Virtual Environment
python -m venv venv

Windows
venv\Scripts\activate

Linux/Mac
source venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt

4. Run the DVC Pipeline
dvc repro

5. Start MLflow
mlflow ui

6. Run Flask Application
python app.py


🧪 Running Tests
pytest


🐳 Docker

-Build the Docker image
docker build -t youtube-sentiment .

-Run the container
docker run -p 5000:5000 youtube-sentiment


📡 API
POST /predict
Request
{
  "comment": "This video is amazing!"
}
Response
{
  "prediction": "Positive"
}


🌐 Chrome Extension

The Chrome Extension allows users to analyze YouTube comments directly from the browser by sending comments to the Flask API and displaying the predicted sentiment in real time.

