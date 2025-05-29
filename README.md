# Transit Delay Prediction 🚦
A machine learning system to predict delays in public transit based on real-time GPS, weather, and route data. Designed for intelligent transport operations.

---
## 🔬 Individual Feature Impact

Explore how each feature influences transit delay predictions:

| Feature | SHAP Dependence Plot |
|---------|----------------------|
| gps_speed | ![gps_speed](figures/shap_gps_speed.png) |
| route_id | ![route_id](figures/shap_route_id.png) |
| weather_code | ![weather_code](figures/shap_weather_code.png) |
| hour | ![hour](figures/shap_hour.png) |

## 🚀 Features
- Predicts delays using historical and real-time features (route ID, GPS, weather)
- Deployed on **AWS Lambda** using **Docker**
- Visualized in **Power BI** for operational monitoring
- Integrated with **SHAP** for model explainability

---

## 🛠 Tech Stack
- **Python**, **Pandas**, **Scikit-learn**
- **AWS Lambda**, **Docker**
- **Power BI**
- **SHAP**

---

## 📊 Use Case
Designed for transit authorities to predict vehicle delays and proactively inform routing and operations teams.

---

## 🔍 SHAP Summary Plot

This plot shows which features most influence the model’s delay predictions:

![SHAP Plot](figures/shap_plot.png)

> 🔵 Blue = Low feature value  🔴 Red = High feature value  
The horizontal axis shows the impact of a feature on the prediction (delay or not).  
The vertical axis lists the most important features:
- **gps_speed**: Speed of the vehicle in km/h
- **route_id**: Transit route number
- **weather_code**: Weather condition (0: Clear, 1: Rain, 2: Snow, 3: Fog)
- **hour**: Hour of the day (from timestamp)

---

## 🔧 Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/your_username/transit-delay-prediction.git
cd transit-delay-prediction
