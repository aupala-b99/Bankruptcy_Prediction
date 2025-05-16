# 🏦 Bankruptcy Risk Prediction | MSBA Financial Group

Hi, I’m Aupala Bhattacharyya! This project is a cloud-native data pipeline I built as part of **GENBUS 780: Cloud Technology for Business Analytics** at the Wisconsin School of Business. It leverages AWS services to predict bankruptcy risk and support investment decision-making—**with no code required**.

---

## 📌 Project Overview

As an analyst for **MSBA Financial Group**, I was responsible for designing a scalable AWS-based architecture to:
- Ingest and transform financial data,
- Store it in a structured warehouse, and
- Generate ML-driven bankruptcy predictions using **SageMaker Canvas**.

The entire pipeline is **built and deployed using AWS-native services**—no Python, SQL, or scripting used.

This project helped me:
- Demonstrate fluency in AWS services like S3, Glue, Redshift, and SageMaker
- Practice presenting cloud-native workflows to non-technical audiences
- Deliver a production-ready pipeline that outputs clear, actionable predictions

---

## 🧰 Tools & Services

| Service             | Purpose                                                      |
|---------------------|--------------------------------------------------------------|
| **Amazon S3**       | Stores raw input files and final prediction outputs          |
| **AWS Glue Studio** | Performs serverless ETL (joins, cleaning, transformation)    |
| **Amazon Redshift** | Warehouses processed financial data for querying             |
| **Amazon SageMaker Canvas** | Trains and deploys machine learning models without code |
| **Canvas Export**   | Generates bankruptcy prediction output as CSV or PNG         |

---

## 🗺 Architecture Overview

Here’s a visual representation of my pipeline from raw files to final predictions:

![AWS Pipeline Architecture](./Picture1.png)

### Process Flow:
1. **Input Files**: CSVs and TXT data are uploaded to an S3 bucket.
2. **Glue ETL**: AWS Glue processes and joins the files into a clean dataset.
3. **Redshift**: The output is stored in a Redshift cluster for easy access.
4. **SageMaker Canvas**: Canvas pulls data from Redshift and trains an ML model.
5. **Predictions**: Bankruptcy scores are exported from Canvas back to S3.

---

## 📁 Data Sources

- `datacorp_financial_data.csv`
- `msba_fg_ratios_data.csv`
- `msba_fg_bankruptcy.txt`
- `company_profiles_to_predict_unlabeled.csv`

These datasets were used to train and score financial entities.

---

## ✅ Recommendations

### 👍 Included in Portfolio:
- Pharmasolve  
- Ninetech  
- Songster Inc  
- Rogers & Sons  
- Hallandall AG  
- Foster & Kruse  
- Highwood & Hart  

### ❌ Excluded from Portfolio:
- Western Corp  
- Design Solutions  
- Innocore  

Prediction outputs were exported from SageMaker Canvas as `.csv` and `.png`.

---

## 🚀 Deployment Highlights

- **Zero Code**: All steps configured via AWS Console
- **ETL Automation**: Done in AWS Glue Studio (visual workflows)
- **ML Modeling**: Built using SageMaker Canvas’ AutoML interface
- **Storage**: Raw and predicted data stored securely in S3
- **Scalable Design**: Redshift and Glue designed to support growing datasets

---

## 🔭 Future Enhancements

- Schedule recurring Glue jobs via triggers or EventBridge
- Use QuickSight to visualize bankruptcy predictions in dashboards
- Deploy model scoring pipelines using SageMaker Pipelines
- Enable stakeholder-friendly access to outputs

---
