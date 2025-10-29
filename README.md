# 🩺 Hadoop Healthcare Analytics

This project implements a **Hadoop-based Healthcare Database System** that integrates **MySQL**, **Sqoop**, **HDFS**, **Hive**, and **Python** for large-scale healthcare data analytics and visualization.

---

## 📘 Project Overview
Healthcare systems generate vast amounts of data daily from hospitals, labs, and monitoring devices.  
Traditional databases struggle to process this volume efficiently.  
Using **Hadoop** and its ecosystem, we can store, process, and analyze healthcare data at scale to extract meaningful insights about patient health and lifestyle factors.

---

## 🧱 Tech Stack
| Tool | Purpose |
|------|----------|
| **MySQL** | Store and manage structured healthcare data |
| **HDFS (Hadoop)** | Distributed storage for large-scale data |
| **Sqoop** | Data transfer between MySQL and Hadoop |
| **Hive** | Querying and aggregating large data in Hadoop |
| **Python (Pandas, Matplotlib, Seaborn)** | Visualization and exploratory data analysis |

---

## 📊 Dataset
- **Source:** [Kaggle – Healthcare Dataset (by Prasad22)](https://www.kaggle.com/datasets/prasad22/healthcare-dataset)
- **Records:** 70,000+ patients
- **Features:**
  - Demographics (age, gender, race)
  - Lifestyle factors (smoking, alcohol, sleep, physical activity)
  - Health indicators (BMI, diabetes, heart disease, stroke)

---

## ⚙️ Implementation Steps

### 1️⃣ MySQL
```sql
CREATE DATABASE healthcare_db;
USE healthcare_db;

CREATE TABLE healthcare_data (
  id INT AUTO_INCREMENT PRIMARY KEY,
  age INT,
  gender VARCHAR(10),
  bmi FLOAT,
  smoking_status VARCHAR(20),
  alcohol_drinking BOOLEAN,
  stroke BOOLEAN,
  physical_activity BOOLEAN,
  sleep_time FLOAT,
  mental_health FLOAT,
  physical_health FLOAT,
  diff_walking BOOLEAN,
  diabetic VARCHAR(20),
  race VARCHAR(30),
  general_health VARCHAR(20),
  asthma BOOLEAN,
  kidney_disease BOOLEAN,
  skin_cancer BOOLEAN,
  heart_disease BOOLEAN
);
