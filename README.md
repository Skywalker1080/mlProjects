# 🧠 Student Performance ML App

This project predicts student exam scores using machine learning and serves the trained model via a Flask web application.

---

## 🚧 Project Overview

- **Model Training**: Conducted in a Jupyter notebook using the `LinearRegression` model from scikit-learn.
- **Web App**: Flask app takes user input (student attributes) and returns predicted scores.
- **Deployment**: Dockerfile included for containerized deployment.


## ⚙️ Setup Instructions

### 1. Clone and Install

```bash
git clone https://github.com/Skywalker1080/ml-test.git
cd ml-test
pip install -r requirements.txt
```

2. Train the Model
Open and run 2. MODEL TRAINING.ipynb to:

Load stud.csv

Preprocess the data

Train the regression model

Save the model as model.pkl

```bash
cd app
python app.py
```

Visit: http://127.0.0.1:5000

# 🐳 Docker Deployment
Build the Image

```bash
docker build -t student-score-app .
```

Run the Container

```bash
docker run -p 5000:5000 student-score-app
```
📌 Notes
Model is trained using features like gender, parental education, test preparation, etc.

Target: Predicting math score.

Predictions are returned via the web UI form.