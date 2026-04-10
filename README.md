#  37 kW Motor Failure Prediction & Risk Analysis  
### ELGi Equipment Limited Internship Project  

---

##  Overview
This project focuses on analyzing field failure data of **37 kW air compressor motors** to enable **predictive maintenance**.  
It combines machine learning and clustering techniques to identify failure patterns and detect at-risk motors before breakdown.

---

##  Problem Statement
Reactive maintenance practices result in:
- Unplanned equipment failures  
- Reduced asset lifespan  
- Increased operational costs  

This highlights the need for a **predictive and data-driven maintenance approach**.

---

##  Objective
To implement predictive maintenance for air compressor motors by:
- Identifying failure patterns  
- Detecting risk zones  
- Improving workflow, product quality, and equipment reliability  

---

##  Dataset Description
- **Source:** ELGi Equipment Limited (Internship Data)  
- **Motor Type:** 37 kW Air Compressor Motors  
- **Records:** 1,484 motors  
- **Features:** 47 parameters  

###  Feature Categories:
- Electrical: Resistance, Voltage, Current  
- Mechanical: Performance indicators  
- Operational: Startup characteristics  

###  Target Variable:
- `1 → Running`  
- `0 → Failed`  

---

##  Data Preprocessing
- Removed non-essential metadata and redundant features  
- Standardized feature names for clarity  
- Filtered only relevant electrical and operational parameters  
- Cleaned missing values  

 Result: A refined dataset suitable for analysis and modeling  

---

##  Workflow

1. 37 kW Motor Dataset  
2. Data Cleaning & Segregation  
3. Univariate Analysis  
4. DBSCAN Clustering  
5. Cluster Visualization  
6. At-Risk Motor Detection

   This workflow ensures systematic analysis from raw data to actionable insights for predictive maintenance.
---

##  Methodology

### 1. Data Cleaning & Segregation
- Removed missing values  
- Split dataset into:
  - Running Motors  
  - Failed Motors  

---

### 2. Feature Analysis
- Performed univariate analysis  
- Identified:
  - Failure thresholds  
  - Outliers  
  - Feature impact on motor failure  

---

### 3. Adaptive DBSCAN Clustering
- Applied DBSCAN on failed motor data  
- Used **dynamic eps (90th percentile distance)**  
- Detected natural failure clusters and outliers  

---

### 4️. Visualization
- Created 1D cluster plots for each feature  
- Displayed:
  - Cluster ranges  
  - Failure percentages  
  - Noise (abnormal cases)  

---

### 5️. Risk Screening
- Compared failure clusters with running motors  
- Identified motors operating in **failure-prone ranges**  

---

##  Results
- DBSCAN identified **failure-critical ranges in 37 out of 46 parameters**  
- **20 parameters showed strong failure zones** requiring monitoring  

###  Example:
- **Resistance_1**:
  - High-risk ranges: `[94.36–97.44]`, `[103.60–104.20]`  
  - Stable range: `[107.91–109.18]`  

 Demonstrates DBSCAN’s effectiveness in detecting motor faults  

---

##  Interpretation
- Identified **stable vs failure-prone operating zones**  
- Some motors fail even at low usage → indicates hidden risks  
- Running motors within failure zones are **at high risk**  

 Enables:
- Early fault detection  
- Improved maintenance planning  
- Increased operational safety  

---

##  Conclusion
- Successfully identified **motor failure zones**  
- Enabled **predictive maintenance strategy**  
- Reduced potential downtime and operational risks  

---

##  Business Impact
- Improves equipment reliability  
- Reduces maintenance cost  
- Supports **lean manufacturing goals**  
- Enhances product quality and workflow efficiency  

---

##  Internship
Developed during 6 months internship at **ELGi Equipment Limited** using real-world industrial data.

---

##  Key Highlight
> This project is based on real industrial data and demonstrates practical application of machine learning in predictive maintenance.
