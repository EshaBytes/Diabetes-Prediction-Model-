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
```
## 🛠️ Installation and Running Locally


# 1. Clone the Repository
```bash
git clone https://github.com/your-username/diabetes-prediction-model.git
cd diabetes-prediction-model
```

# 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate    # For Linux/macOS
# OR
venv\Scripts\activate       # For Windows
```

# 3. Install Dependencies
```bash
pip install -r requirements.txt
```

# 4. Run the Project
```bash
# Train the model
python train_model.py
```

# 5. Start the Flask server
```bash
python server.py
```
Open the frontend:
Open 'frontend/index.html' and click "Go Live" in VS Code
OR open the HTML file manually in your browser



## 📦 Requirements

* Python 3.8+
* Libraries:
  * Flask
  * scikit-learn
  * PyTorch
  * Pandas
  * NumPy
  * Pickle

## 📸 Screenshots

![Screenshot (271)](https://github.com/user-attachments/assets/d46915de-11f9-4cba-b627-ab01f9b5ad0f)
![Screenshot (272)](https://github.com/user-attachments/assets/9da9d639-eb31-4ae5-8d3e-9085a007276b)
![Screenshot (273)](https://github.com/user-attachments/assets/dbb4cb82-5ee8-410f-9c02-5a38912bba61)
![Screenshot (274)](https://github.com/user-attachments/assets/9ad75fb4-be60-475d-9419-ee1e3bc7cf60)
![Screenshot (275)](https://github.com/user-attachments/assets/0f8e410d-6f43-4aa3-8cc4-fc59dab89f13)
