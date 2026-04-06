
# 🧠 Dynamic Health Insurance Premium Prediction using HFS

A **data-driven insurance pricing system** that dynamically adjusts premiums based on **Health + Financial Instability (HFS)** using **temporal modeling and distributed computing (Apache Spark)**.

---

## 🚀 Overview

Traditional insurance models rely on **static features** like age, BMI, and smoking status. This project introduces a **dynamic framework** that:

* Captures **temporal instability (7, 30, 90 days)**
* Combines **health + financial stress signals**
* Generates a **composite HFS score**
* Dynamically adjusts premiums using:

```
Premium = Base Cost × (1 + λ × HFS)
```

📌 The system shifts insurance from **reactive → predictive → adaptive**

---

## 🧩 System Architecture

### 🔹 Workflow Pipeline

<img width="1036" height="444" alt="image" src="https://github.com/user-attachments/assets/22d34088-95cd-47e1-9f5d-b1fa21c1c74f" />

The system is divided into 3 major modules:

### 1️⃣ Dataset Engineering (Kaggle-based)

* Data simulation (health + financial signals)
* Temporal aggregation (7d / 30d / 90d)
* HFS computation
* Base cost prediction (Random Forest)

### 2️⃣ Deployment Simulation (VM + Spark)

* Distributed batch processing (HDFS + Spark)
* Dynamic premium computation
* Temporal alignment & analysis

### 3️⃣ Validation & Analytics

* Model performance evaluation (R²)
* Signal Propagation Gain (SPG)
* Correlation & reporting

---

## ⚙️ Core Concept: HFS Score

The **Health-Financial Stability (HFS)** score is defined as:

```
HFS = α(HV) + β(FV) + γ(AV)
```

Where:

* HV → Health variability
* FV → Financial volatility
* AV → Abnormal signals

📌 Weighted aggregation improves real-world risk modeling.

---

## 📊 Results & Insights

### 🔹 Feature Importance Shift

<img width="854" height="611" alt="image" src="https://github.com/user-attachments/assets/6d303a46-0835-46b2-9f52-d1f56b9507d9" />

* Baseline → dominated by **static cost**
* With HFS → **dynamic instability becomes significant**
* Reduces over-dependence on static attributes

---

### 🔹 Model Performance (R² Improvement)

<img width="854" height="611" alt="image" src="https://github.com/user-attachments/assets/58f2c825-c125-472c-aa94-4ec28ece54af" />

| Window | Baseline | With HFS |
| ------ | -------- | -------- |
| 7-Day  | ~0.80    | ~0.93    |
| 30-Day | ~0.85    | ~0.95    |
| 90-Day | ~0.90    | ~0.97    |

📈 Improvement: **8% – 15% increase in predictive accuracy** 

---

### 🔹 Premium Distribution Analysis

<img width="973" height="689" alt="image" src="https://github.com/user-attachments/assets/178fd55b-ed1f-4702-a327-0b196bc498ff" />

Key observations:

* Right-skewed → most users moderate risk
* Few high-risk → higher premium spikes
* Stable distribution across time windows

---

### 🔹 Premium Stability & Trends

<img width="494" height="378" alt="image" src="https://github.com/user-attachments/assets/4399c616-aed1-4905-9ca0-76995ce65627" />


* Smooth premium transitions
* No abrupt jumps
* Ensures **actuarial stability + adaptability**

---

### 🔹 SPG Metric (Innovation)

We introduce a new metric:

```
SPG = (R²(HFS) - R²(Base)) / (1 - R²(Base))
```

📊 Results:

* 7-Day → **0.713**
* 30-Day → **0.708**
* 90-Day → **0.684**

👉 HFS explains **~68–71% of remaining prediction error** 

---

## 📁 Dataset

📌 Dataset used:

* Based on **Kaggle Medical Cost Dataset**
* Extended with:

  * Financial activity simulation
  * Physiological signals
  * Temporal instability features

👉 **Dataset Link (Google Drive):**
[*DRIVE*](https://drive.google.com/drive/folders/1ar6XasfSQHFu7ebgqhtOjRv_F5rk8Y_v?usp=sharing)

---

## 🛠️ Tech Stack

* **Python (ML + Simulation)**
* **Scikit-learn (Random Forest, XGBoost)**
* **Apache Spark (Distributed Processing)**
* **HDFS (Storage Layer)**
* **NumPy / Pandas / Matplotlib**

---

## 📂 Project Structure

```
├── data/
├── notebooks/
│   └── model.ipynb
├── src/
│   ├── hfs_computation.py
│   ├── premium_engine.py
│   └── spark_pipeline.py
├── results/
│   ├── feature_importance.png
│   ├── model_performance.png
│   ├── premium_distribution.png
│   └── trends.png
└── README.md
```

---

## 🧪 How to Run

```bash
# Clone repo
git clone https://github.com/your-username/hfs-insurance

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook
```

---

## 💡 Key Contributions

✔️ Introduced **HFS (Health + Financial Stress) metric**
✔️ Multi-window temporal modeling (7/30/90 days)
✔️ Distributed premium computation using Spark
✔️ New evaluation metric **SPG**
✔️ Transition from **static → dynamic insurance pricing**

---

## 📌 Future Work

* Real-time streaming (Kafka + Spark Streaming)
* Integration with wearable health devices
* Explainable AI for risk transparency
* Deployment as SaaS insurance engine

---

## 📜 Reference

This work is based on the invention:

**“Dynamic Health Insurance Premium Prediction Using a Combined Health and Financial Stress Score”** 

---

## 👨‍💻 Authors

Kush Arora, Aryan Saxena, Akshat Khandelwal


---


