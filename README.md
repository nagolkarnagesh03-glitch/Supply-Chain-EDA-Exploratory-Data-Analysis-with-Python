# 🚚 Supply Chain EDA – Exploratory Data Analysis with Python

A comprehensive Exploratory Data Analysis (EDA) project on a supply chain dataset, uncovering patterns in revenue, supplier performance, logistics costs, product types, and customer demographics using Python.

---

## 📌 Project Overview

This project performs end-to-end EDA on a real-world-style supply chain dataset (`chain.csv`). It covers data cleaning, univariate/bivariate/multivariate analysis, and business-driven Q&A insights — all visualized with Matplotlib.

---

## 📂 Dataset

| Feature | Description |
|---|---|
| `sku` | Stock Keeping Unit identifier |
| `product_type` | Category of product (e.g., skincare, haircare, cosmetics) |
| `price` | Product selling price |
| `revenue_generated` | Total revenue per product |
| `stock_levels` | Current inventory level |
| `number_of_products_sold` | Units sold |
| `supplier_name` | Name of the supplier |
| `manufacturing_costs` | Cost to manufacture the product |
| `defect_rates` | Rate of defective units |
| `production_volumes` | Volume produced |
| `lead_times` | Time from order to delivery |
| `manufacturing_lead_time` | Manufacturing-specific lead time |
| `shipping_costs` | Cost of shipping |
| `shipping_carriers` | Carrier used for delivery |
| `transportation_modes` | Mode of transport |
| `order_quantities` | Units ordered |
| `availability` | Product availability |
| `location` | Geographic location |
| `customer_demographics` | Customer segment |
| `inspection_results` | Quality inspection outcome |
| `routes` / `costs` | Logistics route and associated cost |

---

## 🛠️ Tech Stack

- **Python 3**
- **Pandas** – data loading, cleaning, groupby, pivot tables
- **NumPy** – numerical operations
- **Matplotlib** – all visualizations (bar, histogram, scatter)
- **Jupyter Notebook** – interactive analysis environment

---

## 📊 Analysis Performed

### 🔹 Data Cleaning
- Standardized column names (lowercase, underscores)
- Verified zero null values and zero duplicates
- Identified numeric vs. categorical columns

### 🔹 Univariate Analysis
- Distribution of product types, prices, revenue, stock levels
- Manufacturing cost, defect rates, production volume distributions
- Lead time, shipping cost, order quantity distributions

### 🔹 Bivariate Analysis
- Price vs. Revenue (scatter)
- Price vs. Number of Products Sold
- Stock Level vs. Sales
- Availability vs. Revenue
- Lead Time vs. Shipping Cost
- Production Volume vs. Revenue
- Manufacturing Cost vs. Defect Rate

### 🔹 Group-Level Analysis
- Average revenue & price by product type
- Supplier frequency and manufacturing cost comparison
- Defect rate by supplier
- Shipping cost by carrier and transportation mode
- Revenue by customer demographics and location
- Production volume by supplier

### 🔹 Multivariate / Pivot Analysis
- Supplier × Product Type → Revenue, Manufacturing Cost, Defect Rate
- Shipping Carrier × Transportation Mode → Shipping Cost
- Location × Product Type → Revenue
- Supplier × Shipping Carrier → Shipping Cost

### 🔹 Business Q&A (10 Key Questions)
| # | Question |
|---|---|
| Q1 | Which supplier generates the highest total revenue? |
| Q2 | Which product type is the most profitable? |
| Q3 | Which supplier has the highest defect rate? |
| Q4 | Which shipping carrier has the highest average shipping cost? |
| Q5 | Which transportation mode is the most cost-effective? |
| Q6 | Which products should be restocked first? (Low Stock + High Sales) |
| Q7 | Which suppliers have high manufacturing costs but low revenue? |
| Q8 | Which routes contribute the highest logistics costs? |
| Q9 | Which product type has the best inventory turnover? |
| Q10 | Which customer demographic generates the highest revenue? |

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/supply-chain-eda.git
cd supply-chain-eda
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib jupyter
```

### 3. Run the Notebook
```bash
jupyter notebook "supply_chain_eda.ipynb"
```

> ⚠️ Make sure `chain.csv` is in the same directory as the notebook before running.

---

## 📁 Project Structure

```
supply-chain-eda/
│
├── supply_chain_eda.ipynb   # Main Jupyter Notebook
├── chain.csv                # Dataset (add manually)
└── README.md                # Project documentation
```

---

## 💡 Key Insights

- **Revenue leaders:** Certain SKUs and supplier-product combinations consistently outperform others in revenue.
- **Defect risk:** Defect rates vary significantly by supplier — a critical factor for quality control decisions.
- **Logistics optimization:** Transportation mode and carrier choice directly impact shipping costs.
- **Restock alerts:** Several high-selling products show dangerously low stock levels.
- **Inventory turnover:** Product types differ in how efficiently they convert stock into sales.

---

## 👨‍💻 Author

**[Nagesh Nagolkar]**  
📧 nagolkarnagesh03@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) | [GitHub](https://github.com/your-username)

---




**💼 4 Strong ATS Resume Points**

Replace placeholders with your actual figures once you run the notebook.

1. Conducted end-to-end Exploratory Data Analysis on a 1,000+ row supply chain dataset using Python (Pandas, NumPy, Matplotlib), uncovering supplier defect patterns and revenue drivers across 20+ variables.
   
3. Built 30+ visualizations (histograms, bar charts, scatter plots, pivot heatmaps) to analyze pricing strategy, logistics costs, and customer demographics — identifying top-performing supplier-product combinations by revenue.

5. Engineered an inventory turnover metric and applied multi-criteria sorting to flag high-priority restocking SKUs with low stock and high sales volume, enabling data-driven supply chain decisions.

7. Performed multivariate analysis using Pandas pivot tables across Supplier × Product Type × Transportation Mode dimensions to compare manufacturing costs, defect rates, and shipping efficiency across the supply chain.
