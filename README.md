# 📊 Olist E-Commerce Analysis: Retention Leak Case Study

## 🔍 Overview
This project is a deep-dive analysis of a Brazilian e-commerce marketplace dataset (Olist) to understand a critical business problem: **low customer retention**.

Despite generating significant revenue, the platform was struggling to convert first-time buyers into repeat customers.

Using **Excel, Power Query, and Data Modeling**, I transformed 9+ raw relational tables into a structured dataset and uncovered a key insight:

> 🚨 **87% of customers never returned after their first purchase.**

---

## 🎯 Problem Statement

The business showed strong top-line performance:

- 💰 **Total GMV:** R$15.8M  
- 📦 **100,000+ orders processed**

However, a deeper look revealed a structural issue:

> Growth was driven by **new customers**, not **repeat customers**

### Key Questions:
- Why are customers not returning?
- Is this a marketing problem or an operational problem?
- What factors influence customer satisfaction and retention?

---

## 📂 Dataset Source

- 📊 **Olist E-Commerce Dataset (Kaggle)**
- Includes:
  - Orders
  - Customers
  - Sellers
  - Reviews
  - Products
  - Geolocation

⚠️ **Note:**  
Due to file size limitations, raw datasets and working files are not uploaded to this repository.

However:
- Dataset source is linked above  
- Full analysis process is documented here  
- Visual outputs are included via screenshots  

---

## 🛠️ Tools & Techniques

- **Excel**
- **Power Query (ETL)**
- **Data Modeling (Relational Structure)**
- **DAX (Calculated Metrics)**
- **PivotTables & Dashboards**

---

## 🧠 Analysis Framework

To ensure accuracy and scalability, I followed a structured 5-step workflow:

### 1. Define the Grain
- Established **one row per order item**
- Prevented ambiguity before joins

---

### 2. Sanitize at Source
- Cleaned and transformed individual tables before merging
- Examples:
  - Aggregated reviews at `order_id` level  
  - Removed duplicate geolocation entries  

---

### 3. Validate Every Join
- Performed **row-count audits after each merge**
- Prevented:
  - Data duplication  
  - Inflated revenue  
  - Incorrect metrics  

---

### 4. Feature Engineering (Decision Metrics)

Created meaningful business metrics:

- **SLA Breach Flag** → Did delivery exceed estimated date?  
- **Delivery Duration** → Purchase → Delivery timeline  
- **Sentiment Buckets** → Positive / Neutral / Negative reviews  

---

### 5. Stakeholder-Focused Visualization

Designed dashboards for different business functions:

- 📊 Executive (Strategy)
- ⚙️ Operations (Logistics)
- 💬 Customer Experience

---

## 🔗 Core Insight (Causal Chain)
