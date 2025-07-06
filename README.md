# 📊 IT Expenditure Analysis Dashboard – Power BI Project

## 🔍 Project Overview

This project focuses on analyzing and monitoring IT expenditure across multiple business units, regions, and IT functional areas. It was developed using Power BI and provides a unified dashboard to compare **Actual**, **Forecast**, and **Planned** IT spending — helping stakeholders make data-driven budgeting and investment decisions.

---

## 🎯 Problem Statement

Large organizations often struggle to monitor IT spending effectively due to distributed operations and siloed data.  

**Core question:**  
> How can the organization monitor and optimize IT expenditures across departments, geographies, and categories to improve financial governance and strategic alignment?

---

## 💡 Objective

- Track and compare **Actual vs Forecast vs Plan** for IT costs  
- Identify **variance trends** and spending inefficiencies  
- Visualize spend distribution across **regions**, **business units**, and **IT areas**  
- Enable **interactive filtering** to support multiple stakeholder views  

---

## 🗂️ Dataset Description

The dataset includes:

| Column             | Description                                 |
|--------------------|---------------------------------------------|
| Date               | Month-wise IT spend records                 |
| Actual             | Actual IT cost incurred                     |
| Forecast           | Forecasted IT cost                          |
| Plan               | Planned IT budget                           |
| IT_Area            | Functional domain of IT spend               |
| Business_Area      | Business unit where cost was incurred       |
| Region             | Geographical region                         |
| Cost_Element_Group | IT cost category (e.g., labor, services)    |

---

## 🧪 Data Preparation & Transformation (in Power BI)

- **Null handling** for missing values in Actual, Forecast, and Plan columns  
- **Data type conversion** for date and currency columns  
- **Custom date table** to sort and visualize months correctly  
- **DAX Measures** created for:
  - `Variance Amount` = Actual – Plan  
  - `Variance %` = (Actual – Plan) / Plan  
  - `Forecast Accuracy` = (Actual – Forecast) / Forecast  
- **Relationships** defined between dimension tables and the main fact table  
- **Filtering logic** applied to exclude zero or incomplete rows  

---

## 📊 Dashboard Features

The Power BI report contains the following visuals:

1. **Top KPIs**  
   - Total Actual, Forecast, Plan  
   - Variance % and Variance Amount  

2. **Monthly Trend Charts**  
   - Clustered Column and Line Charts for Actual, Forecast, and Plan  

3. **Donut Chart by IT Area**  
   - Visualizes Actual spend by IT function  

4. **Bar Chart by Region**  
   - Compares Actual spend across global regions  

5. **Interactive Filters**  
   - Slicers for Region, Business Area, IT Area, and Cost Element Group  

---

## 📷 Dashboard Preview

![Dashboard Screenshot](https://github.com/sravangowrigari/IT-Expenditure-Analysis/blob/main/Screenshot%202025-07-06%20175300.png)

---

## 📈 Key Insights

- Actual spend was **~$34M under budget** (–3.77% variance)  
- **Functional IT**, **BU Support**, and **Infrastructure** make up over 90% of the spending  
- **USA** accounts for the majority of IT expenses, while other regions lag behind  
- Year-end spike in December may indicate delayed or bulk spending  
- Governance and Enablement functions appear underfunded  

---

## 🛠️ Tools Used

- **Power BI Desktop**  
- Power Query for data transformation  
- DAX for measure calculations  
- Excel for source data  

---

## 📁 File Structure

📂 IT-Expenditure-Analysis/
1. IT_Expenditure_Analysis.pbix # Main Power BI dashboard file
2. IT Expenditure dataset.xlsx # Source dataset
3. Screenshot.png # Dashboard screenshot
4. README.md # Project overview and documentation

## 📌 How to Use

1. Download the `IT_Expenditure_Analysis.pbix` file.
2. Open in **Power BI Desktop**.
3. Load the Excel dataset if not already embedded.
4. Use the slicers on the left to explore region-wise or function-wise insights.
5. Share as report or export visuals for stakeholder presentations.

---

## 📬 Contact

**Author:** Sravan Gowrigari  
📧 For queries or collaborations, reach out via GitHub or email.
