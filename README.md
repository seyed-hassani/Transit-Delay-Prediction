# Transit Delay Prediction 🚦

A machine learning system to predict public transit delays using real-time data.

## 🚀 Features
- Predicts delays using GPS, weather, and route data.
- AWS Lambda deployment with containerized packaging.
- Power BI dashboard to visualize delay likelihoods.
- SHAP integration for model explainability.

## 🛠 Tech Stack
- Python, Pandas, Scikit-learn
- AWS Lambda, Docker
- Power BI
- SHAP

## 🔧 How It Works
1. Input: Route ID, GPS logs, weather status, timestamp
2. Output: Delay classification (on-time vs delayed)
3. Updates Power BI in real-time for operational teams

## ⚙️ Setup
```bash
git clone https://github.com/your_username/transit-delay-prediction.git
cd transit-delay-prediction
pip install -r requirements.txt
python train_model.py
