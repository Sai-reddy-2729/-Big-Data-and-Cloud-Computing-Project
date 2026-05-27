# -Big-Data-and-Cloud-Computing-Project


# 🚀 Big Data and Cloud Computing Project  
## AWS-Based Scalable Data Processing & Machine Learning Pipeline  

---

## 📌 Project Overview  

This project demonstrates an end-to-end **Big Data and Cloud Computing solution** using AWS services.  
It processes large-scale datasets (≥1GB) using distributed computing and applies data engineering and machine learning techniques to extract insights.

The pipeline follows a complete lifecycle:

**Data Ingestion → Cloud Storage → Distributed Processing → Data Cleaning → Feature Engineering → Machine Learning → Analytics → Visualization**

---

## 🎯 Objective  

To design and implement a scalable cloud-based big data architecture that:

- Handles large-scale datasets efficiently  
- Uses Apache Spark for distributed processing (AWS EMR)  
- Stores data securely in Amazon S3  
- Performs analytics using AWS Athena and Glue  
- Builds machine learning models for prediction  
- Visualizes insights using Power BI  

---

## 📊 Dataset Information  

- Dataset Type: Large-scale Review / Accidents / Text dataset  
- Size: Greater than 1GB  
- Format: JSON / CSV → Converted to Parquet  
- Source: Kaggle / AWS Open Data / Public Dataset  

### Key Features:
- User ID  
- Product / Business ID  
- Ratings / Severity  
- Review Text  
- Timestamp  
- Sentiment Label  
- Location / Weather attributes (if applicable)  

---

## ☁️ AWS Cloud Services Used  

- Amazon S3 → Storage (raw + processed data)  
- Amazon EMR → Distributed processing (Apache Spark)  
- AWS Glue → Schema & metadata catalog  
- Amazon Athena → Serverless SQL queries  
- IAM → Security and access control  
- Power BI → Data visualization  

---

## 🏗️ Architecture Flow  


Data Source
↓
Amazon S3 (Raw Data Storage)
↓
Amazon EMR (Spark Processing)
↓
Data Cleaning + Feature Engineering
↓
Parquet Files Stored in S3
↓
AWS Glue Data Catalog
↓
Amazon Athena SQL Queries
↓
Power BI Dashboard Visualization


---

## ⚙️ Data Processing Steps  

### 1. Data Ingestion  
- Dataset downloaded from public source  
- Uploaded to Amazon S3  
- Connected to EMR using IAM roles  

---

### 2. Data Cleaning (PySpark)  
- Removed null values  
- Removed duplicates  
- Converted text to lowercase  
- Removed special characters using regex  
- Handled missing values  

---

### 3. Feature Engineering  
- Tokenization of text  
- Stopword removal  
- Review length calculation  
- Sentiment labeling (positive / negative / neutral)  

---

## 🤖 Machine Learning Model  

### Algorithm Used:
- Logistic Regression / Random Forest Classifier  

### Workflow:
- Train-Test Split (80/20)  
- Feature extraction using TF-IDF / OneHotEncoding  
- Model training  
- Evaluation using Accuracy & F1 Score  

### Evaluation Metrics:
- Accuracy  
- F1 Score  
- Confusion Matrix  

---

## 📈 Data Analysis & Insights  

Using Amazon Athena and Spark:

- Average rating analysis  
- Sentiment distribution  
- Top reviewed products  
- Customer behavior patterns  
- Time-based trends  

---

## 📊 Power BI Dashboard  

The dashboard includes:

- Total Reviews KPI  
- Average Rating  
- Sentiment Distribution  
- Review Length Analysis  
- Rating Distribution Charts  

---

## 💰 Cost Optimization Strategies  

- Used Parquet format (reduces storage cost)  
- S3 lifecycle policies implemented  
- EMR clusters terminated after job completion  
- Athena used for serverless pay-per-query model  

---

## 🔐 Security & Compliance  

- IAM role-based access control  
- S3 bucket permission restrictions  
- Data encryption (at rest & in transit)  
- Secure EMR access using SSH key pairs  

---

## 📡 Performance Monitoring  

- EMR cluster monitoring using Spark logs  
- Athena query performance tracking  
- S3 storage monitoring  
- Debugging via log analysis  

---

## 📁 Project Structure  


Big-Data-Cloud-Project/
│
├── etl_pipeline.py
├── ml_pipeline.py
├── data_ingestion.py
├── requirements.txt
├── README.md
│
├── datasets/
├── outputs/
│ ├── parquet/
│ ├── models/
│ └── visualizations/
│
└── screenshots/


---

## 🚀 How to Run  

### Step 1: Clone Repository

git clone https://github.com/your-username/repo-name.git


### Step 2: Install Dependencies

pip install -r requirements.txt


### Step 3: Run ETL Pipeline

python etl_pipeline.py


### Step 4: Run ML Model

python ml_pipeline.py


---

## 🧰 Technologies Used  

- Python  
- Apache Spark (PySpark)  
- AWS S3  
- AWS EMR  
- AWS Glue  
- Amazon Athena  
- Scikit-learn  
- Power BI  

---
