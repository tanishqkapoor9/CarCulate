# 🚗 Car Price Prediction

A **machine learning-powered web application** that predicts used car prices based on multiple input features such as **year, mileage, fuel type, transmission, and brand**. The project combines **data preprocessing, feature engineering, regression modeling, and a Flask web app** to provide real-time predictions.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue" />
  <img src="https://img.shields.io/badge/Flask-Framework-green" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Regression-yellow" />
  <img src="https://img.shields.io/badge/Scikit--Learn-ML%20Library-red" />
</p>

---

## 📹 Video Demo
[(*Insert screenshots of your app here*)](https://github.com/user-attachments/assets/e97abd0e-e7c2-4900-92db-35ad1299b2d4)


---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Framework:** Flask (for serving ML model via web app)
* **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Pickle
* **Frontend:** HTML, CSS (integrated with Flask templates)

---

## ⚙️ Features

* Predicts car price based on multiple real-world factors.
* **Data preprocessing pipeline** with handling for categorical, numerical, and missing values.
* **Feature engineering**: One-hot encoding, scaling, and transformations.
* **Regression modeling** using Linear Regression (with option to extend to Random Forest, Gradient Boosting, etc.).
* Web app built with **Flask** to make predictions user-friendly.
* Model serialized with **Pickle** for deployment.

---

## 📊 Machine Learning Pipeline

1. **Data Collection**

   * Dataset of used cars with attributes like `year`, `present_price`, `kms_driven`, `fuel_type`, `seller_type`, `transmission`, `owner`, etc.

2. **Data Preprocessing**

   * Missing value handling
   * Label encoding for categorical features (`Fuel_Type`, `Seller_Type`, `Transmission`)
   * Feature scaling with `StandardScaler`

3. **Feature Engineering**

   * Derived `Car Age` feature from manufacturing year
   * Removed multicollinear features

4. **Model Training**

   * Trained **Linear Regression** model as baseline
   * Evaluated with **R² score, MAE, RMSE**
   * Experimented with **ensemble models** (RandomForest, GradientBoosting) for performance benchmarking

5. **Model Deployment**

   * Serialized best model using `pickle`
   * Integrated into a **Flask backend** with an HTML form UI

---

## 📈 Results

* Achieved an **R² score of \~0.85** on test data.
* Predictions closely match market values within reasonable error bounds.

---

## 🚀 Installation & Usage

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/car-price-prediction.git
cd car-price-prediction
```

### 2️⃣ Create Virtual Environment & Install Dependencies

```bash
python -m venv venv
source venv/bin/activate   # for Mac/Linux
venv\Scripts\activate      # for Windows

pip install -r requirements.txt
```

### 3️⃣ Run the Flask App

```bash
python application.py
```

Navigate to `http://127.0.0.1:5000` in your browser.

---

## 📂 Project Structure

```
Car-Price-Prediction/
│── data/                     # Dataset(s)
│── notebooks/                # Jupyter notebooks (EDA, model training)
│── static/                   # CSS, JS, Images
│── templates/                # HTML templates for Flask
│── application.py            # Flask entry point
│── model.pkl                 # Serialized ML model
│── requirements.txt          # Dependencies
│── README.md                 # Project documentation
```

---

## 🔮 Future Improvements

* Add support for **multiple ML models** with model comparison.
* Deploy on **Heroku / AWS / Render** for public access.
* Integrate a **REST API endpoint** for programmatic access.
* Enhance UI with React/Next.js frontend.

---

## 👨‍💻 Author

**Tanish Kapoor**
🔗 [LinkedIn](https://linkedin.com/in/tanishkapoor) | [GitHub](https://github.com/tanishkapoor)

---


