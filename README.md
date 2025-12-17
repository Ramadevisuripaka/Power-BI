<!doctype html>
<h3>Filled Map</h3>
<div class="example">Filled map</div>
<div class="meta">Usage: fills regions to indicate intensity. Good for state / country-level KPIs.</div>
</article>


<article class="card">
<h3>Slicer</h3>
<div class="example">Slicer control</div>
<div class="meta">Usage: interactive filter for dashboards (date, category, region).</div>
</article>


<article class="card">
<h3>Number Card</h3>
<div class="example">Card — single value</div>
<div class="meta">Usage: highlight a single metric, e.g. Total Sales, % Growth, or Count.</div>
</article>


<article class="card">
<h3>Stacked Bar Chart</h3>
<div class="example">Stacked bar</div>
<div class="meta">Usage: compare composition across categories (horizontal orientation).</div>
</article>


<article class="card">
<h3>Stacked Column Chart</h3>
<div class="example">Stacked column</div>
<div class="meta">Usage: compare composition across categories (vertical orientation).</div>
</article>


<article class="card">
<h3>Clustered Bar Chart</h3>
<div class="example">Clustered bar</div>
<div class="meta">Usage: compare groups side-by-side across categories (horizontal).</div>
</article>


<article class="card">
<h3>Clustered Column Chart</h3>
<div class="example">Clustered column</div>
<div class="meta">Usage: compare groups side-by-side across categories (vertical).</div>
</article>


<article class="card">
<h3>100% Stacked Bar / Column</h3>
<div class="example">100% stacked</div>
<div class="meta">Usage: show percentage composition where each bar/column sums to 100%.</div>
</article>


</div>
</section>


<section style="margin-top:20px">
<h2 style="margin:0 0 10px">How to use this page</h2>
<div class="card">
<ol style="margin:0 0 8px;padding-left:18px">
<li>Replace the placeholder images with exported images from Power BI desktop (File → Export → PNG).</li>
<li>Update the text descriptions with your learning outcomes or data sources.</li>
<li>Commit this file as <code>index.html</code> into a GitHub repository to publish via GitHub Pages (optional).</li>
</ol>
<div class="meta">Tip: Keep each visualization accompanied with a one-line insight (e.g., "Region X had 32% of total sales in Q1").</div>
</div>
</section>


<footer>
<div>
<a class="btn btn-primary" href="#" onclick="alert('Replace with your GitHub repo link')">View on GitHub</a>
<a class="btn btn-ghost" href="#" onclick="alert('Replace with link to Power BI file or screenshot folder')">Download PBIX / Screenshots</a>
</div>
<div style="color:var(--muted);font-size:0.92rem">Created: Power BI — 1 week class project</div>
</footer>
</div>
</body>
</html>
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>Power BI — Class Notes</title>
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <style>
    /* Clean, readable styling */
    body { font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial; line-height:1.5; margin:0; padding:24px; background:#fbfdff; color:#0b1220; }
    header { display:flex; gap:16px; align-items:center; margin-bottom:18px; }
    h1 { margin:0; font-size:28px; }
    .tag { background:#e6f0ff; color:#003a8c; padding:6px 10px; border-radius:999px; font-size:13px; }
    .meta { color:#495057; font-size:13px; }
    nav { margin: 18px 0; padding:12px; background:#fff; border:1px solid #e6ebf2; border-radius:8px; }
    nav a { display:inline-block; margin-right:12px; color:#0366d6; text-decoration:none; }
    section { margin-top:20px; padding:18px; background:white; border:1px solid #eef2f7; border-radius:10px; }
    h2 { margin-top:0; }
    .example { font-size:14px; padding:10px; background:#fbfbff; border-radius:6px; border:1px dashed #e5e9f2; margin-top:8px; }
    ul { margin:8px 0 12px 20px; }
    code { background:#f6f8fa; padding:2px 6px; border-radius:4px; font-family: monospace; }
    footer { margin-top:28px; font-size:13px; color:#6b7280; }
    .grid { display:grid; gap:12px; grid-template-columns: repeat(auto-fit,minmax(240px,1fr)); }
    .card { padding:12px; border-radius:8px; background:#fff; border:1px solid #eef2f7; }
  </style>
</head>
<body>
  <header>
    <div>
      <h1>Power BI — Class Notes</h1>
      <div class="meta">Summary of visuals, analyses & tools learned — ready for GitHub</div>
    </div>
    <div style="margin-left:auto" class="tag">Power BI</div>
  </header>

  <nav>
    <strong>Contents:</strong>
    <a href="#types-of-analysis">Types of analysis</a>
    <a href="#columns">Types of columns</a>
    <a href="#scatter">Scatter plot</a>
    <a href="#line">Line chart</a>
    <a href="#include-exclude">Include / Exclude</a>
    <a href="#tables">Table / Matrix</a>
    <a href="#others">Other visuals</a>
  </nav>

  <section id="types-of-analysis">
    <h2>Types of analysis</h2>
    <p>Short descriptions of common analysis approaches in Power BI:</p>
    <ul>
      <li><strong>Exploratory analysis:</strong> Look for patterns & anomalies using visuals (scatter, tree map).</li>
      <li><strong>Comparative analysis:</strong> Compare categories (column, stacked bar, line & column).</li>
      <li><strong>Trend analysis:</strong> Use time-series visuals (line chart) to see trends over time.</li>
      <li><strong>Root-cause analysis:</strong> Drill-down using hierarchies, matrix and filters.</li>
    </ul>
    <div class="example">Tip: Start with simple visuals, then add slicers/filters to narrow insights.</div>
  </section>

  <section id="columns">
    <h2>Types of columns</h2>
    <ul>
      <li><strong>Text (string)</strong>: categories, names.</li>
      <li><strong>Numeric</strong>: integers, decimals — used for sums, averages.</li>
      <li><strong>Date/Time</strong>: use for trend/time-series and hierarchies (year, month).</li>
      <li><strong>Calculated columns</strong>: row-level derived values via DAX.</li>
      <li><strong>Measures</strong>: aggregation-level calculations (SUM, AVERAGE, custom DAX).</li>
    </ul>
    <div class="example">Example DAX measure: <code>Total Sales = SUM(Sales[Amount])</code></div>
  </section>

  <section id="scatter">
    <h2>Scatter plot</h2>
    <p>Used to show relationship between two numerical measures. You can also add size and color to represent additional dimensions.</p>
    <ul>
      <li><strong>X-axis:</strong> numeric measure (e.g., Unit Price)</li>
      <li><strong>Y-axis:</strong> numeric measure (e.g., Quantity Sold)</li>
      <li><strong>Size:</strong> Market Size or Sales Amount</li>
      <li><strong>Color:</strong> Category to group points</li>
    </ul>
    <div class="example">Use scatter when you want to spot clusters, correlation, or outliers.</div>
  </section>

  <section id="outliers">
    <h2>Outliers</h2>
    <p>Points far from the main cluster — investigate causes (data errors, special events, real anomalies).</p>
    <ul>
      <li>Filter the chart or use <code>Top N</code> filters to highlight outliers.</li>
      <!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>Power BI — Class Notes</title>
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <style>
    body { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial; background:#f7fafc; color:#0b1220; margin:0; padding:28px; }
    .container { max-width:1000px; margin:0 auto; }
    header { display:flex; align-items:center; gap:16px; margin-bottom:18px; }
    h1 { margin:0; font-size:28px; }
    .badge { margin-left:auto; background:#e6f0ff; color:#0447a6; padding:6px 10px; border-radius:999px; font-size:13px; }
    nav { margin:16px 0; padding:12px; background:#fff; border:1px solid #e6ebf2; border-radius:8px; }
    nav a { margin-right:12px; color:#0366d6; text-decoration:none; }
    section { background:#fff; border:1px solid #eef2f7; border-radius:10px; padding:16px; margin-bottom:14px; }
    h2 { margin-top:0; }
    ul { margin:8px 0 12px 18px; }
    .tip { background:#fbfbff; padding:10px; border-radius:6px; border:1px dashed #e5e9f2; fon
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Power BI - Power Query & Transform Data</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            margin: 20px;
            background-color: #f9f9f9;
            color: #333;
        }
        h1, h2, h3 {
            color: #0b5394;
        }
        .container {
            background: #ffffff;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        ul {
            margin-left: 20px;
        }
        code {
            background: #eee;
            padding: 3px 6px;
            border-radius: 4px;
        }
        .footer {
            margin-top: 30px;
            text-align: center;
            font-size: 14px;
            color: #666;
        }
    </style>
</head>
<body>

<div class="container">

    <h1>Power BI – Power Query & Transform Data</h1>
    <p><strong>Topic:</strong> Power Query Editor & Home Tab Functions</p>
    <p><strong>Tool:</strong> Microsoft Power BI</p>

    <hr>

    <h2>📌 What is Power Query?</h2>
    <p>
        Power Query is a data transformation and data preparation tool in Power BI.
        It helps to clean, shape, and transform raw data into a usable format
        before loading it into the Power BI model.
    </p>

    <h2>📌 Transform Data</h2>
    <p>
        The <strong>Transform Data</strong> option opens the Power Query Editor.
        It allows users to perform data cleaning and transformation steps such as:
    </p>
    <ul>
        <li>Removing unnecessary columns</li>
        <li>Filtering rows</li>
        <li>Changing data types</li>
        <li>Splitting and merging columns</li>
        <li>Handling missing or duplicate values</li>
    </ul>

    <h2>📌 Power Query Home Tab Functions</h2>

    <h3>1️⃣ Close & Load</h3>
    <p>
        Applies all transformations and loads the cleaned data into Power BI.
    </p>

    <h3>2️⃣ New Source</h3>
    <p>
        Used to connect to new data sources like Excel, CSV, SQL Server, Web, etc.
    </p>

    <h3>3️⃣ Recent Sources</h3>
    <p>
        Quickly access previously used data sources.
    </p>

    <h3>4️⃣ Manage Parameters</h3>
    <p>
        Create and manage parameters for dynamic and reusable queries.
    </p>

    <h3>5️⃣ Data Source Settings</h3>
    <p>
        Modify permissions and credentials of connected data sources.
    </p>

    <h3>6️⃣ Refresh Preview</h3>
    <p>
        Refreshes the data preview to reflect latest changes.
    </p>

    <h3>7️⃣ Choose Columns</h3>
    <p>
        Select only required columns and remove unwanted columns from the dataset.
    </p>

    <h3>8️⃣ Remove Columns</h3>
    <p>
        Delete selected or unselected columns from the table.
    </p>

    <h3>9️⃣ Keep Rows</h3>
    <p>
        Keep top rows, bottom rows, or specific range of rows.
    </p>

    <h3>🔟 Remove Rows</h3>
    <p>
        Remove top rows, bottom rows, blank rows, or duplicate rows.
    </p>

    <h3>1️⃣1️⃣ Sort</h3>
    <p>
        Sort data in ascending or descending order.
    </p>

    <h3>1️⃣2️⃣ Transform</h3>
    <p>
        Perform column-level transformations such as:
    </p>
    <ul>
        <li>Change data type</li>
        <li>Format text</li>
        <li>Split column</li>
        <li>Replace values</li>
    </ul>

    <h3>1️⃣3️⃣ Combine</h3>
    <p>
        Merge or append queries to combine multiple tables.
    </p>

    <h2>📌 Conclusion</h2>
    <p>
        Power Query is a powerful tool for data cleaning and transformation.
        Understanding Power Query Home tab functions helps in preparing high-quality
        data for analysis and visualization in Power BI.
    </p>

    <div class="footer">
        <p>📘 Created for learning & GitHub documentation purposes</p>
        <p>🚀 Power BI | Power Query | Data Transformation</p>
    </div>

</div>

</body>
</html>
# 📊 Power BI Visualization Assignment

## 📌 Project Title

**Sales, Profit, and Units Analysis using Power BI**

---

## 🧠 Project Overview

This project focuses on analyzing business performance data using **Power BI**. The dataset contains sales-related information such as **Sales**, **Profit**, **Units Sold**, **Manufacturing Price**, **Sales Price**, **Discount Band**, and **Time (Date)**.

The goal of this assignment is to:

* Understand sales and profit trends over time
* Analyze the impact of discounts on profit
* Study the relationship between manufacturing cost, sales price, and profit
* Create clear and meaningful visualizations for business insights

---

## 🗂️ Dataset Used

* **File Name:** Financial Sample.xlsx
* **Source:** Sample financial dataset (used for learning & analysis)

### Key Columns:

* Date
* Sales
* Profit
* Units Sold
* Manufacturing Price
* Sales Price
* Discount Band
* Country / Segment (if available)

---

## 🛠️ Tools & Technologies

* **Power BI Desktop** – Data cleaning, modeling, and visualization
* **Power Query** – Data transformation
* **GitHub** – Project documentation and sharing

---

## 🔄 Step-by-Step Workflow

### Step 1: Data Import

* Open Power BI Desktop
* Click **Get Data → Excel**
* Load `Financial Sample.xlsx`

### Step 2: Data Cleaning (Power Query)

* Checked data types
* Removed unnecessary columns
* Renamed columns for better understanding
* Verified null or blank values

### Step 3: Data Modeling

* Ensured correct relationships
* Verified numeric and date fields

---

## 📈 Visualizations Created

### 1️⃣ Time-Based Trend Analysis

**Objective:** Understand business performance over time

* Monthly Sales Trend (Line Chart)
* Quarterly Profit Trend (Line Chart)
* Yearly Units Sold Trend (Column Chart)

📌 *Insight:* Sales and profit show seasonal patterns and steady growth in certain periods.

---

### 2️⃣ Discount Impact Analysis

**Objective:** Analyze how discount bands affect sales and profit

* Sales by Discount Band (Column Chart)
* Profit by Discount Band (Bar Chart)

📌 *Insight:* Higher discounts increase sales volume but reduce profit margins.

---

### 3️⃣ Manufacturing Price vs Sales Price vs Profit

**Objective:** Understand cost and pricing impact on profit

* Scatter Plot: Manufacturing Price vs Profit
* Scatter Plot: Sales Price vs Profit

📌 *Insight:* Profit increases when the gap between sales price and manufacturing price is higher.

---

### 4️⃣ Relationship Between Key Metrics

**Objective:** Identify correlation among Sales, Profit, and Units Sold

* Scatter Chart: Sales vs Profit
* Scatter Chart: Units Sold vs Profit

📌 *Insight:* Higher units sold generally lead to higher sales, but profit depends on pricing and discounts.

---

## 🎯 Key Learnings

* Time-based analysis helps identify trends and seasonality
* Discounts directly affect profitability
* Pricing strategy plays a crucial role in profit generation
* Power BI visuals make data-driven decisions easier

---

## 📁 Project Structure (GitHub)

```
PowerBI-Visualization-Assignment/
│
├── Dataset/
│   └── Financial Sample.xlsx
│
├── PowerBI_File/
│   └── Financial_Analysis.pbix
│
├── Screenshots/
│   └── dashboard_images.png
│
└── README.md
```

---

## 🚀 How to View the Project

1. Download the `.pbix` file
2. Open it using **Power BI Desktop**
3. Explore different report pages and interact with visuals

---

## 🙌 Conclusion

This assignment helped me gain hands-on experience in **data visualization**, **business analysis**, and **Power BI reporting**. The project demonstrates how raw data can be transformed into meaningful insights using effective visual storytelling.

---

📌 *Created by:* **Ramadevi Suripaka**
📅 *Tool Used:* Power BI Desktop




