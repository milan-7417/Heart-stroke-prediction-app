<h1 align="center">🫀 Heart Stroke Prediction Web App</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.13.5-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" height="45"/>
  <img src="https://img.shields.io/badge/Streamlit-1.25-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" height="45"/>
  <img src="https://img.shields.io/badge/Scikit--learn-1.3-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn" height="45"/>
  <img src="https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" height="45"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" height="45"/>
  <img src="https://img.shields.io/badge/Docker%20Hub-Image%20Registry-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Hub" height="45"/>
  <img src="https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=white" alt="Render" height="45"/>
</p>

A user-friendly machine learning web application that predicts the likelihood of **heart stroke** based on key health and demographic indicators.

The application uses a trained **Logistic Regression** model to generate predictions from user-provided health information and provides an intuitive interface built with **Streamlit**.

The application has been **Dockerized and deployed on Render**, making it available as a containerized web service.

---

## 📌 Project Overview

Stroke is a serious health condition where early identification of potential risk factors can be valuable.

This project demonstrates how a machine learning model can be integrated into an interactive web application to estimate stroke risk based on user-provided health indicators.

The application allows users to enter relevant health information and receive a prediction instantly.

> ⚠️ **Disclaimer:** This application is intended for educational and demonstration purposes only. It is not a medical diagnostic tool and should not be used as a substitute for professional medical advice.

---

## ✨ Features

* **Interactive User Interface** — Simple and intuitive Streamlit interface for entering health information.
* **Machine Learning Prediction** — Uses a trained Logistic Regression model to predict stroke risk.
* **Real-Time Inference** — Generates predictions immediately after submitting the input.
* **User-Friendly Design** — Designed for users without a technical background.
* **Containerized Deployment** — Packaged into a Docker image for consistent and reproducible deployment.
* **Cloud Deployment** — Docker container deployed and running on Render.

---

## 🛠️ Technology Stack

### 🐍 Programming & Machine Learning

* **Python 3.13.5**
* **Scikit-learn 1.3**
* **Pandas**
* **Joblib**
* **Logistic Regression**

### 🎨 Frontend & Application

* **Streamlit 1.25**

### 📊 Data Analysis & Visualization

* **Jupyter Notebook**
* **Matplotlib**
* **Seaborn**

### 🐳 Deployment & Infrastructure

* **Docker**
* **Docker Hub**
* **Render**

---

## 🏗️ Application Architecture

```text
                         User
                          │
                          ▼
                 ┌─────────────────┐
                 │   Render Cloud  │
                 │                 │
                 │  Docker         │
                 │  Container      │
                 │       │         │
                 │       ▼         │
                 │   Streamlit     │
                 │       │         │
                 │       ▼         │
                 │  ML Prediction  │
                 │       │         │
                 │       ▼         │
                 │ Logistic        │
                 │ Regression      │
                 └─────────────────┘
                          │
                          ▼
                  Stroke Risk Result
```

### Deployment Workflow

```text
Source Code
     │
     ▼
 Dockerfile
     │
     ▼
 Docker Image
     │
     ▼
 Docker Hub
     │
     ▼
 Render
     │
     ▼
 Running Docker Container
     │
     ▼
 Streamlit Web Application
```

---

## 🐳 Dockerization

The application is packaged using Docker to provide a consistent and reproducible runtime environment containing the application code, Python environment, dependencies, and trained model.

The container:

1. Uses a Python base image.
2. Sets the application working directory.
3. Copies the project files into the container.
4. Installs dependencies from `requirements.txt`.
5. Exposes the Streamlit port.
6. Starts the Streamlit application.

The application runs with:

```bash
streamlit run app.py
```

---

## ☁️ Deployment on Render

The application is deployed on **Render as a Docker-based web service**.

The Docker image is deployed as a running container, which serves the Streamlit application to users over the web.

```text
GitHub Repository
        │
        ▼
    Dockerfile
        │
        ▼
   Docker Image
        │
        ▼
    Docker Hub
        │
        ▼
      Render
        │
        ▼
 Docker Container
        │
        ▼
 Streamlit Application
```

---

## 💻 Run Locally Without Docker

### Prerequisites

* Python 3.9+
* Git

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/<your-repository>.git
cd <your-repository>
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate on Windows:

```bash
venv\Scripts\activate
```

On macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py
```

The application will typically be available at:

```text
http://localhost:8501
```

---

## 🐳 Run Using Docker

### 1. Build the Docker Image

```bash
docker build -t heart-stroke-prediction .
```

### 2. Run the Container

```bash
docker run -p 8501:8501 heart-stroke-prediction
```

### 3. Open the Application

Visit:

```text
http://localhost:8501
```

---

## 📁 Project Structure

```text
heart-stroke-prediction/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── model/
│   └── model.pkl
│
├── notebooks/
│   └── analysis.ipynb
│
├── dataset/
│   └── dataset.csv
│
└── README.md
```

> The exact structure may vary depending on the files included in the repository.

---

## 🤖 Machine Learning Model

The application uses **Logistic Regression** as the prediction model.

```text
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Feature Processing
     │
     ▼
Model Training
     │
     ▼
Logistic Regression
     │
     ▼
Model Serialization
     │
     ▼
Streamlit Application
```

---

## 🔮 Prediction Workflow

```text
User Input
    │
    ▼
Input Validation
    │
    ▼
Feature Preparation
    │
    ▼
Trained Logistic Regression Model
    │
    ▼
Prediction
    │
    ▼
Stroke Risk Result
```

---

## 🚀 Future Improvements

* Improve UI/UX and visualizations.
* Add automated model retraining.
* Implement CI/CD for automated Docker builds and deployments.
* Add comprehensive model evaluation metrics.

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

**Milan Kumar**

If you found this project useful or interesting, consider ⭐ starring the repository.
