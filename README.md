# 🌍 IoT Air Quality Monitoring & Sensor Calibration System

## 🚀 Project Overview
This project presents a **real-world IoT air quality monitoring system** combined with **machine learning-based sensor calibration** to improve the reliability of low-cost air quality sensors.

The system collects and analyses environmental data from **low-cost, mid-cost, and high-cost (reference-grade) sensors**, comparing their performance and applying models to enhance accuracy.

---

## 🎯 Key Objectives
- Build a **scalable IoT-based air quality monitoring system**
- Compare **low-cost vs mid-cost vs reference sensors**
- Improve low-cost sensor accuracy using **machine learning calibration**
- Analyse **sensor reliability in real-world urban environments**
- Provide insights for **cost-effective smart city deployments**

---

## 🏙️ Deployment Locations
- **Node 3:** QMUL Mile End Road (Urban roadside traffic)
- **Node 5:** King Edward Memorial Park (Urban roadside traffic)

📍 Sensors were **co-located (<1m apart)** to ensure fair comparison.

---

## 📊 Data Overview
- **Collection Period:** April – July 2025 (3 months)
- **Sampling Frequency:**
  - Low/Mid-cost sensors: **30 seconds**
  - Reference stations: **15 minutes**
- **Pollutants Measured:**
  - PM2.5, PM10
  - NO₂, CO, O₃
  - VOC Index
  - Temperature & Humidity

---

## 🧠 Machine Learning & Data Processing

### 🔧 Data Engineering
- Merged multi-source datasets with **different sampling rates**
- Built pipelines using:
  - `Pandas`, `NumPy`
- Handled:
  - Missing values
  - Time alignment
  - Sensor inconsistencies

---

### 🤖 Models Used
- Linear Regression  
- Polynomial Regression  
- Random Forest Regressor  

---

## 📈 Key Results
| Pollutant | Performance | Insight |
|----------|------------|--------|
| **PM2.5** | ⭐ Strong (r ≈ 0.83) | Highly reliable & calibratable |
| **NO₂** | ⚠ Moderate (r ≈ 0.58) | Noisy but usable |
| **CO** | ⚠ Moderate (~0.49) | Needs calibration |
| **O₃** | ❌ Poor (~0.05) | Unreliable due to cross-sensitivity |

✅ Achieved **R² up to 0.72** for calibrated PM2.5 models  
⚠ Identified **sensor drift & cross-node performance degradation**

---

## 🔍 Key Insights
- Low-cost PM2.5 sensors can be **significantly improved using ML calibration**
- Some sensors (e.g. ozone) are **not suitable for accurate measurement**
- Sensor performance varies across environments → **generalisation is challenging**
- **Cost-effective monitoring is possible** with the right calibration strategy

---

## 🛠️ Tech Stack

**Languages & Libraries**
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib / Seaborn

**Concepts**
- Time-Series Analysis  
- Machine Learning Regression  
- Sensor Calibration  
- IoT Data Processing  

## 📊 Example Analysis
- Correlation matrices across sensor types  
- Time-series comparisons (low vs reference)  
- Cross-node validation (generalisation testing)  

---

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/Abisco96/Improving-Accuracy-of-Low-Cost-Air-Quality-Sensors-Using-Calibration-Techniques.git

# Install dependencies
pip install -r requirements.txt

# Run analysis notebook
jupyter notebook
```
---
## 📂 Repository Structure
```bash
├── node_3/
│   ├── low_cost/
│   ├── mid_cost/
│   └── high_cost/
├── node_5/
│   ├── low_cost/
│   ├── mid_cost/
│   └── high_cost/
├── data_dictionary.md
├── deployment_details.csv
├── sensor_specifications.csv
└── README.md
```
##  📊 Example Analysis
Correlation matrices across sensor types
Time-series comparisons (low vs reference)
Cross-node validation (generalisation testing)

## 💡 Why This Project Matters

Most air quality systems rely on expensive reference stations.

This project shows that:

➡️ Low-cost sensors can be reliable with calibration

➡️ Cities can deploy scalable and affordable monitoring networks

➡️ Data + ML + IoT = real-world impact


# Install dependencies
pip install -r requirements.txt

# Run analysis notebook
[Updated Low-cost Air Quality Sensor Calibration to improve their data quality.ipynb](https://github.com/Abisco96/Improving-Accuracy-of-Low-Cost-Air-Quality-Sensors-Using-Calibration-Techniques/blob/main/Updated%20Low-cost%20Air%20Quality%20Sensor%20Calibration%20to%20improve%20their%20data%20quality.ipynb)

## 🖼 Demo
https://drive.google.com/file/d/12q_E3AJbOoQqVGMTiYqINQUerdcoG31U/view?usp=sharing

## 👩🏽‍💻 Author
Abigail Frimpong

MSc Graduate – IoT & Data Analytics

Passionate about IoT, Data Science, and Smart Cities

Interested in Software Engineering, Data, and Embedded Systems roles

## ⭐ Final Note

This project demonstrates a unique combination of:

Real-world IoT deployment

Data engineering

Machine learning

Analytical thinking


👉 Few graduates have this full stack — this is what sets this work apart.
