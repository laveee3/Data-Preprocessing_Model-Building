# Data Preprocessing & Model Building

This repository demonstrates **data cleaning, preprocessing, and machine learning model development** using two real-world use cases:  
1. **Power trading organization data preparation**  
2. **Auto-insurance claim prediction model**

---

##  Project Overview

### **1. Data Preparation & Preprocessing (Power Trading Organization)**

We received **hourly weather metrics** and **power output values (kWh)** datasets from a power trading organization.  
The goal is to clean and prepare the raw data for modeling.

#### **Datasets**
- `Power_data_preprocessing.csv`
- `Weather_data_preprocessing.csv`

#### **Tasks & Constraints**
- Handle missing weather data appropriately and document reasoning.  
- Create categorical variables for time-based features (day, month, or season).  
- Apply an appropriate scaling method for numerical features.  
- Filter out days with **power outages** (wind ≥ 30 mph).  

---

### **2. Model Building (Auto-Insurance Claim Prediction)**

An auto-insurance company needs to build a **pricing model** based on customers' likelihood of filing a claim within their first year.

#### **Dataset**
- `claim_prediction.csv`  
- Contains **10,000 customers** and **10 engineered features** related to driving behavior.  
- Target variable:  
  - `CLAIM = 1`: customer filed a claim  
  - `CLAIM = 0`: customer did not file a claim  

#### **Tasks**
- Build two models:  
  1. For customers **likely to file a claim**  
  2. For customers **unlikely to file a claim**  
- Dataset is pre-cleaned: no missing data, balanced classes, and features already scaled.  

---

##  Notebook Highlights: DataWrangling_ModelBuilding.ipynb

The core notebook **[`DataWrangling_ModelBuilding.ipynb`](DataWrangling_ModelBuilding.ipynb)** covers:

### **Data Wrangling**
- Importing and merging multiple datasets  
- Handling missing data with different imputation strategies  
- Filtering and cleaning based on domain constraints (e.g., removing outage days)  
- Creating new **categorical and temporal features**  

### **Exploratory Data Analysis (EDA)**
- Summary statistics and correlation analysis  
- Visualizing distributions and relationships using **Matplotlib & Seaborn**  

### **Feature Engineering & Scaling**
- One-hot encoding and ordinal variables  
- Normalization and standardization methods  

### **Model Building**
- Splitting datasets into training and testing sets  
- Building classification models using **scikit-learn**  
- Evaluating models with metrics:  
  - Accuracy, Precision, Recall, F1-score  
  - ROC-AUC and confusion matrix  

### **Visualization**
- Feature importance plots  
- Performance comparison charts across models  

---

##  Tech Stack

- **Languages:** Python (3.x)  
- **Libraries:**  
  - `pandas` – data manipulation  
  - `matplotlib`, `seaborn` – visualization  
  - `scikit-learn` – model building & evaluation  

---

##  Repository Structure

Data-Preprocessing-Model-Building/

├── data/
│ ├── Power_data_preprocessing.csv
│ ├── Weather_data_preprocessing.csv
│ └── claim_prediction.csv

├── notebooks/
│ └── DataWrangling_ModelBuilding.ipynb

├── output/
│ ├── cleaned_power_data.csv
│ ├── weather_summary.csv
│ └── claim_model_results.csv

└── README.md
