# NEXACORE — Intelligent Energy-Aware Data Center Optimizer

> AMD Slingshot Project | Team Leader: A. Rajender Reddy

---

## 🚀 Overview

NEXACORE is an AI-powered energy optimization system for AMD-based data centers. It predicts future workload demand using machine learning and dynamically allocates CPU/GPU resources to minimize power consumption — all while maintaining SLA compliance.

---

## 🧠 Key Features

| Feature | Description |
|---|---|
| 📊 ML Workload Prediction | Time-series forecasting using Ridge Regression with lag features |
| ⚙️ Energy-Aware Allocation | Dynamically allocates CPU cores & GPU units based on predicted load |
| 🌍 Carbon Emission Estimator | Calculates CO₂ saved, cost savings, and tree equivalents |
| 📈 Real-Time Dashboard | Streamlit dashboard with live metrics, charts, and forecast table |
| ✅ SLA Compliance | Maintains 15% headroom above predicted demand at all times |

---

## 🏗️ Project Structure

```
nexacore/
├── data/
│   └── generate_data.py        # Simulated server workload data generator
├── models/
│   └── predictor.py            # ML workload forecasting model
├── modules/
│   ├── resource_allocator.py   # Energy-aware resource allocation engine
│   └── carbon_estimator.py     # Carbon emission & cost savings estimator
├── dashboard/
│   └── app.py                  # Streamlit dashboard (main entry point)
├── requirements.txt
└── README.md
```

---

## ⚙️ Tech Stack

- **Language:** Python 3.9+
- **ML/Data:** Scikit-Learn, NumPy, Pandas
- **Dashboard:** Streamlit + Plotly
- **Optimization:** Custom constraint-based allocator
- **Target Hardware:** AMD EPYC CPUs, AMD Instinct GPUs

---

## 🔧 Installation & Run

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/nexacore.git
cd nexacore

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the dashboard
streamlit run dashboard/app.py
```

The dashboard will open at `http://localhost:8501`

---

## 📸 Dashboard Sections

1. **Live Server Status** — Real-time CPU, GPU, memory, power metrics
2. **AI Resource Allocation** — Gauge charts for CPU/GPU/power allocation
3. **Workload Forecast** — Historical data + ML-predicted future load
4. **Weekly Power Analysis** — NEXACORE vs static scheduler comparison
5. **Carbon Estimator** — CO₂ savings, cost savings, trees equivalent
6. **Allocation Schedule** — Upcoming resource plan table

---

## 🌍 Impact

- Reduces power consumption vs traditional static schedulers
- Estimates annual CO₂ savings and electricity cost reduction
- Designed to align with AMD EPYC and AMD Instinct GPU architectures

---

## 📄 License

MIT License — Free to use and modify.
