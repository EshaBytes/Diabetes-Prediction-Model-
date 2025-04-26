# 🩺 Diabetes Prediction Model

## Overview
This project implements a **Diabetes Prediction System** that uses **Ridge Regression** to predict whether a person has diabetes based on diagnostic measurements.  
The backend is built with **PyTorch** and **scikit-learn**, served via a **Flask** API, and the frontend is designed using **HTML, CSS, and JavaScript** for an interactive user experience.

---

## Features
- Predicts diabetes likelihood based on user inputs.
- Ridge Regression model for robust prediction with regularization.
- Backend REST API using Flask.
- Clean and responsive frontend built with HTML/CSS/JavaScript.
- Model saved in `.pkl` format for easy loading.
- Lightweight and easy to deploy.

---

## Tech Stack
- **Machine Learning:** PyTorch, scikit-learn
- **Backend:** Flask
- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Deployment Ready:** Can be hosted on platforms like Heroku, Render, or AWS.

---

## Dataset
- **Dataset Used:** Pima Indians Diabetes Dataset  
  - Contains medical predictor variables (like BMI, insulin level, age, pregnancies) and one target variable (Outcome: 0 = No Diabetes, 1 = Diabetes).
  - Commonly available via Kaggle or UCI Machine Learning Repository.

---

## How it Works

1. **Data Preprocessing**
   - Load and clean dataset.
   - Apply feature scaling (Standardization).
   - Split into training and testing sets (typically 80:20).

2. **Model Training**
   - Implement Ridge Regression using scikit-learn.
   - Tune hyperparameters (`alpha`) if needed.
   - Save the trained model as `model.pkl` using `pickle`.

3. **Backend (Flask App)**
   - Create API endpoints.
   - Load the `model.pkl` and predict based on user inputs.
   - Return prediction result as JSON.

4. **Frontend**
   - Collect user inputs through a web form.
   - Send data to Flask backend via AJAX.
   - Display prediction results dynamically on the webpage.

---

## Folder Structure
```bash
├── app.py              # Flask backend
├── model.pkl           # Saved Ridge Regression model
├── static/
│   ├── style.css       # Frontend CSS
├── templates/
│   ├── index.html      # Frontend HTML
├── script.js           # Frontend JavaScript
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation
