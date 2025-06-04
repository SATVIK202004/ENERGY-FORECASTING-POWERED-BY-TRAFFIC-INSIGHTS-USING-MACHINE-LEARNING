
# ⚡ Energy Forecasting Powered by Traffic Insights

A machine learning project that enhances urban energy demand forecasting by integrating **real-time traffic data**, **weather conditions**, and **historical energy usage**, using a suite of advanced ML models including **LSTM**, **Random Forest**, and others. This project is aligned with **Sustainable Development Goal 7 (SDG-7)** — access to reliable, affordable, sustainable energy.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Architecture](#architecture)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Modeling Approaches](#modeling-approaches)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [How to Run](#how-to-run)
- [Future Work](#future-work)
- [Contributors](#contributors)

---

## 🌐 Overview

Traditional energy forecasting methods often fail to keep up with **dynamic urban patterns**, such as traffic congestion, seasonality, and sudden anomalies. This project bridges that gap by:

- **Incorporating traffic data as a feature**
- **Applying AI-driven feedback loops**
- **Using cloud-based platforms (AWS SageMaker)** for scalable ML operations

---

## 🚀 Key Features

- 🔄 **Real-time adaptive model tuning**
- 🔍 **Anomaly detection** in energy/traffic patterns
- 🌦️ **Multivariate forecasting** using weather, traffic, and energy datasets
- 🧠 **Comparative model benchmarking** (LR, RF, DT, SVR, LSTM)
- ☁️ **Cloud scalability** with AWS S3 & SageMaker

---

## 🏗️ Architecture

```
Raw Data (Traffic + Energy + Weather)
        ↓
Data Cleaning & Preprocessing
        ↓
Feature Engineering (Peak Hours, Seasonality)
        ↓
Model Training (5 Models)
        ↓
Evaluation & Comparison
        ↓
AI Tuning & Real-Time Feedback Loop
        ↓
Live Energy Demand Forecast
```

---

## 🧾 Dataset

- `traffic.csv` – traffic volume data (hourly, seasonal trends)
- `energy.csv` – historical urban energy consumption
- `weather.csv` – weather conditions mapped to time/date
- **Source**: [Kaggle Datasets](https://www.kaggle.com/)

---

## 🛠 Technologies Used

| Category           | Tools/Technologies              |
|-------------------|---------------------------------|
| ML Models         | LSTM, Random Forest, SVR, etc.  |
| Cloud Platform    | AWS S3, AWS SageMaker           |
| Programming Lang. | Python                          |
| Libraries         | NumPy, pandas, scikit-learn, Keras, matplotlib |
| Visualization     | Matplotlib, Seaborn             |

---

## 🤖 Modeling Approaches

1. **Linear Regression** – Baseline for trend analysis.
2. **Random Forest** – Best performer (92% accuracy); handles nonlinearity.
3. **Decision Tree Regressor** – Quick estimation with interpretable rules.
4. **Support Vector Regressor (SVR)** – Effective for smaller datasets.
5. **LSTM** – Captures temporal dependencies and long-term patterns.

---

## 📊 Evaluation Metrics

| Metric   | Purpose                            |
|----------|-------------------------------------|
| MAE      | Mean Absolute Error                 |
| RMSE     | Root Mean Square Error              |
| R² Score | Model’s goodness-of-fit (accuracy)  |

---

## 📈 Results

| Model         | Accuracy / R² Score |
|---------------|---------------------|
| Linear Reg.   | ~74%                |
| Random Forest | **92%** ✅           |
| Decision Tree | ~88%                |
| SVR           | ~85%                |
| LSTM          | ~90%                |

> Random Forest + LSTM showed best performance and scalability.

---

## 💻 How to Run

1. **Clone the repo**  
```bash
git clone https://github.com/yourusername/energy-forecast-traffic.git
cd energy-forecast-traffic
```

2. **Install dependencies**  
```bash
pip install -r requirements.txt
```

3. **Run the preprocessing script**  
```bash
python preprocess.py
```

4. **Train the model**  
```bash
python train_model.py --model random_forest
```

5. **Visualize results**  
```bash
python visualize_results.py
```

> For LSTM, ensure a GPU environment is used.

---

## 📌 Future Work

- Add **reinforcement learning** for adaptive energy control
- Integrate **real-time APIs** for traffic/weather updates
- Implement **explainable AI** (XAI) dashboards
- Strengthen **cybersecurity** for smart grid systems

---

## 👨‍💻 Contributors

- **P. Venkat Satvik**
- **Sk. Nooruddin**
- **SD Riyaz**
- **G. V. Ramana Reddy** *(Supervisor)*
