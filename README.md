> # **eda_ml_processmining_analysis**
> ### End-to-end process mining, EDA, and ML analysis on case/process data in Python


# Process Mining & Data Analysis Project

## Overview
This repository presents a comprehensive study on process exploration, data analysis, and machine learning modeling. Analyses are conducted from two main perspectives:

- **Process & Data Exploration (including EDA in Python)**  
- **Machine Learning Modeling (ML in Python)**  

**Dataset Columns:**  
`case_id`, `activity`, `start_timestamp`, `event_number`, `resource`, `originator`, `issue_type`, `effort_hours`, `estimated_hours`, `resolved_date`  

**Included Files:**  
- `sample_process_mining_20rows.xlsx` – sample dataset with 20 rows  
- `eda_process_my_data_report.py` – code for process exploration and EDA  
- `ml_my_data_report.py` – code for machine learning modeling  

---

## 1. Process & Data Exploration (including EDA in Python)
<details>
<summary>Click to expand EDA & Process Analysis Contents</summary>

**Goal:** Understand the dataset, uncover patterns, evaluate process performance, and identify bottlenecks.

**Contents:**  
- Import & Load Data  
  - Convert timestamps  
- Basic Data Quality Checks  
  - Missing values  
  - Duplicates  
- Compute Case Duration (Throughput Time)  
- Exploratory Data Analysis (EDA)  
  - Number of cases & activities  
  - Event distribution  
  - Events per case (case size)  
  - Waiting time between consecutive events  
  - Average waiting time per activity  
  - Workload analysis (resource & originator)  
  - Issue-type analysis  
  - Sequence (variant) analysis  
  - Case duration distribution  
  - Monthly case arrivals  
  - SLA analysis  
- Deeper-layer Analysis  
  - Cases sharing the same start timestamp (throughput, originators, resources)  
  - Cases with min/max throughput in groups  
- Bottleneck Analysis  
  - Activity-level, Resource-level, Originator-level, Case-level  
  - Rework & Activity Transition Bottlenecks  
  - Month-over-Month Bottleneck Trends  
- Monthly Summary Table  
  - Most involved features per month

</details>

---

## 2. Machine Learning Modeling (ML in Python)
<details>
<summary>Click to expand ML Contents</summary>

**Goal:** Recognize patterns in data and make predictions.

**Contents:**  
- Import & Load Data  
- Case Features Overview  
- Predictive Analytics  
  - Predict throughput time (regression)  
  - Predict likelihood of rework (classification)  
  - Predict case issue type (classification)  
- Process Mining & Clustering  
  - Case clustering by process behavior  
  - Resource clustering by workload  
- Anomaly Detection  
  - Identify potential bottlenecks  
- Sequence Modeling  
  - Predict mode: "Next Activity"

</details>

---

## Usage
1. Load the **sample dataset**: `sample_process_mining_20rows.xlsx`  
2. Run the Python scripts:  
   - `eda_process_my_data_report.py` for EDA and process mining insights  
   - `ml_my_data_report.py` for predictive modeling  
3. Implemented in **Python**, using:  
   - `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `TensorFlow/Keras`

---

