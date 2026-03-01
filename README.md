# 📊 Retail Performance & Market Expansion For A Global Superstore | Power BI

**Author:** Van Bat Phuc Tai  
**Tools: **Power BI**

---

## 📑 Table of Contents
- [📌 Background & Overview](#-background--overview)  
- [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
- [🧠 Design Thinking Process](#-design-thinking-process)  
- [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
- [🔎 Final Conclusion & Recommendation](#-final-conclusion--recommendation)  

---

## 📌 Background & Overview  

### 🎯 Objective  

Developed a **Power BI dashboard** using the Global Superstore dataset (Orders, People, Returns) to transform transactional data into **actionable business insights** for strategic decision-making.  

The project focuses on:  

- Evaluating overall **sales and profitability performance**  
- Identifying **high-potential markets for expansion**  
- Prioritizing **profitable and scalable product categories**  
- Supporting **ROI-driven decision-making**  

---

### 👤 Target Users  

- Data Analysts & Business Analysts  
- Sales & Marketing teams  
- Route-to-Market & Strategy teams  

---

### ❓ Key Business Questions  

- What is the current performance baseline?  
- Which markets show the strongest growth and ROI potential?  
- Which products should be prioritized for strategic investment?  

---

### 🎯 Project Outcome  

Revenue scaled steadily, but **margin expansion remained constrained**, indicating operational cost pressure.  

Several regions demonstrated **strong margin quality and growth momentum**, highlighting expansion opportunities.  

Technology led revenue performance, though **return-heavy SKUs impacted profitability**. High-margin categories outperformed, while weaker segments diluted overall results.  

This analysis supports alignment between **market expansion strategy, product portfolio optimization, and profitability improvement**.  

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  

- Source: Kaggle  
- Format: CSV  
- ~51K transaction records (Orders table)  

### 📊 Data Structure  

The dataset consists of three relational tables:  

🛒 Orders – Contains detailed transaction and customer information (51,290 records).

<details>
<summary><strong>Table 1: Orders</strong></summary>

| Column Name   | Data Type | Description |
|--------------|----------|------------|
| Order ID     | VARCHAR  | Unique identifier for each order. |
| Order Date   | DATE     | Date when the order was placed. |
| Ship Date    | DATE     | Date when the order was shipped. |
| Ship Mode    | VARCHAR  | Shipping method used for delivery. |
| Customer ID  | VARCHAR  | Unique identifier for each customer. |
| Customer Name| VARCHAR  | Full name of the customer. |
| Segment      | VARCHAR  | Customer segment (e.g., Consumer, Corporate). |
| City         | VARCHAR  | City where the order was placed. |
| State        | VARCHAR  | State where the order was placed. |
| Country      | VARCHAR  | Country where the order was placed. |
| Postal Code  | VARCHAR  | Postal code of the shipping address. |
| Market       | VARCHAR  | Market region (e.g., APAC, EMEA). |
| Region       | VARCHAR  | Geographical region of the order. |
| Product ID   | VARCHAR  | Unique identifier for each product. |
| Category     | VARCHAR  | Product category (e.g., Furniture, Office Supplies). |
| Sub-Category | VARCHAR  | Sub-category of the product. |
| Product Name | VARCHAR  | Name of the product ordered. |
| Sales        | DECIMAL  | Revenue generated from the order. |
| Quantity     | INT      | Number of items ordered. |
| Profit       | DECIMAL  | Profit earned from the order. |

</details>

🔄 Returns – Stores data on returned orders.

<details>
<summary><strong>Table 2: Returns</strong></summary>

| Column Name | Data Type | Description |
|-------------|----------|------------|
| Returned    | VARCHAR  | Indicates whether the order was returned (e.g., 'Yes' or 'No'). |
| Order ID    | VARCHAR  | Unique identifier for each order. |

</details>

👥 People – Holds information about sales representatives.

<details>
<summary><strong>Table 3: People</strong></summary>

> 👥 Holds information about sales representatives.

| Column Name | Data Type | Description |
|-------------|----------|------------|
| Person      | VARCHAR  | Name of the salesperson. |
| Region      | VARCHAR  | Geographic region where the salesperson operates. |

</details>
