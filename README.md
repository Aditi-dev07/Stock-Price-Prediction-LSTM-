---

# 📈 LSTM-Based Stock Price Forecasting (RELIANCE.NS)

A deep learning time-series forecasting project that predicts the **next-day closing price** of Reliance Industries using an **LSTM neural network built with PyTorch**.

> 🎓 Developed as a self-learning academic project to gain hands-on experience in real-world machine learning workflows.

---

## 🧠 Project Motivation

As a student exploring **Deep Learning for Time-Series**, this project was created to:

* Understand how stock market data behaves
* Learn how to properly preprocess sequential data
* Implement LSTM using PyTorch
* avoid common mistakes like **data leakage**
* build a complete end-to-end ML pipeline

This project focuses on **learning and implementation**, not financial trading.

---
## 📊 Dataset

* **Source:** Yahoo Finance
* **Stock:** RELIANCE.NS
* **Duration:** 9 Years
* **Interval:** 1 Day

### Features used:

* Open
* High
* Low
* Close
* Volume

### Target:

Next-day closing price

---

## 🏗️ Project Workflow

### 1️⃣ Data Preprocessing

* Chronological train-test split
* MinMax scaling (fit only on training data)
* No shuffling (time-series aware)

### 2️⃣ Sequence Creation

Transforming time-series into supervised learning format:

```
Previous N days → Next day Close
```

### 3️⃣ Model Development

* Custom PyTorch Dataset & DataLoader
* LSTM architecture
* MSE loss function
* Adam optimizer

### 4️⃣ Evaluation Metrics

* MAE
* RMSE
* R² Score

### 5️⃣ Visualization

* Training loss curve
* Actual vs Predicted prices

---

## 📈 Results

* R² Score: **~0.88 – 0.90**

The high R² is mainly due to **price autocorrelation**, which is expected in
next-day price prediction.

This project demonstrates:

✅ Correct time-series validation
✅ No data leakage
✅ Proper scaling and inverse transformation

---

## ⚠️ Important Note

This model predicts **price movement continuity**, not a trading strategy.

The goal of this project is to showcase:

* Deep learning skills
* Time-series handling
* PyTorch implementation

---

## 🛠️ Tech Stack

* Python
* PyTorch
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* yFinance

---

## 📂 Project Structure

```
├── LSTM.ipynb
├── README.md
├── requirements.txt
```

---

## ▶️ How to Run

```bash
git clone https://github.com/your-username/lstm-stock-forecasting.git
cd lstm-stock-forecasting
pip install -r requirements.txt
```

Open:

```
LSTM.ipynb
```

---

## 🚀 What I Learned

* Handling sequential data for deep learning
* Avoiding data leakage in time-series
* Building LSTM in PyTorch from scratch
* Model evaluation for regression problems
* Importance of baseline comparison
* Writing clean, reproducible ML code

---

## 🔮 Future Improvements

* Compare with naive baseline
* Predict returns instead of raw price
* Hyperparameter tuning
* Walk-forward validation
* Multi-step forecasting
* Transformer-based models

---

## 👨‍💻 Author

**Aditi Verma**
Postgraduate Student 
Aspiring **Data Scientist | ML Engineer**

---

## ⭐ Why this project matters

This repository highlights my ability to:

* Learn complex concepts independently
* Use AI tools like ChatGPT effectively
* Build real-world ML projects
* Follow best practices in time-series modeling

---

# 💬 Recruiter Note

This is a **learning-focused project** that demonstrates strong fundamentals in:

* Deep Learning
* PyTorch
* Time-Series Forecasting
* ML project structuring
