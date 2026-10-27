# Online Store Sales & Customer Analysis

**Python | Data cleaning | Sales analysis | Customer segmentation**

If I was working with a small online store, I would start with a simple question: **What is selling, and which customers are coming back?**

This is a practice project where I cleaned retail order data, focused on the online sales channel, created charts, and wrote a short report with recommendations.

> **Practice project, not client work.** The data is synthetic and the findings describe this sample only. I did not work with a real store or real customer records.

## What I worked on

- Checked for duplicates, missing values, invalid quantities, and returned orders.
- Cleaned the order data and focused on the **Online** sales channel.
- Compared monthly sales, product categories, and regions.
- Grouped identified customers into **one-time**, **repeat**, and **top repeat** customers using simple, explained rules.
- Prepared an Excel workbook, four charts, and a two-page PDF summary.

## Main findings

| Metric | Result |
|---|---:|
| Original retail records | 612 |
| Exact duplicate rows found | 12 |
| Valid non-returned online orders analyzed | 175 |
| Online sales revenue | 126,657.37 dataset units |
| Average online order value | 723.76 dataset units |
| Identified online customers | 106 |
| One-time customers | 59 |
| Repeat customers, including top repeat | 47 |

**Electronics** has the highest online sales revenue in the sample, making up **71.7%** of online revenue. The highest monthly revenue happened in **June 2026**. The dataset does not specify a currency, so I have not labeled the amounts as dollars or pounds.

## Charts

**Monthly online sales**

![Monthly online sales](charts/01_monthly_sales.png)

**Sales by category**

![Sales by category](charts/02_category_sales.png)

**Sales by region**

![Sales by region](charts/03_region_sales.png)

**Customer buying groups**

![Customer buying groups](charts/04_customer_groups.png)

## Project files

| File | What it contains |
|---|---|
| [Jupyter notebook](notebooks/online_store_sales_analysis.ipynb) | The Python code, explanations, tables, and charts |
| [Short PDF report](deliverables/Sales_Analysis_Report.pdf) | Key numbers, four charts, and three recommendations |
| [Cleaned Excel workbook](deliverables/Cleaned_Online_Store_Sales.xlsx) | Summary, cleaned online sales, and customer groups |
| [Case study](PROJECT_SUMMARY.md) | The problem, approach, findings, and limitations |
| [Input data](data/) | Three synthetic practice CSVs: orders, products, and customers |
| [Analysis outputs](outputs/) | CSV exports and a results JSON file |

## How to run

1. Download or clone this repository.
2. Open the folder in **VS Code**.
3. Install the packages:

   ```bash
   pip install -r requirements.txt
   ```

4. Open `notebooks/online_store_sales_analysis.ipynb` and run the cells from top to bottom.

The notebook also works in Jupyter Notebook. It reads the CSV files from the `data/` folder and recreates the charts and outputs. The saved notebook includes real executed outputs so the work can be viewed directly on GitHub.

## Three ideas I would discuss with a store owner

1. Review stock and profit margins for the highest-revenue products before planning promotions.
2. Test a follow-up campaign for one-time customers, with appropriate marketing consent, and measure repeat orders.
3. Compare website traffic and promotions with slower sales months to find out what caused the difference.

**Important limitations:** Returned orders are excluded from the revenue shown here; refunds have not been independently reconciled. Records without a customer ID still count in sales, but not customer segmentation. No improvement in business revenue is claimed.
