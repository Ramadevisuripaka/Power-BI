# 📘 Power BI & Power Query – Complete Beginner Learning Notes

> **Learning Period:** From **December 1st** till now
> **Learner:** Ramadevi Suripaka
> **Purpose:** Self-learning + Beginner-friendly GitHub documentation

---

## 📌 Introduction

This repository contains **step-by-step learning notes** of **Power BI** and **Power Query**, written in **simple human language** for **absolute beginners**.

The goal of this documentation is:

* To clearly explain **each topic I learned**
* To explain **every important tool in Power BI**
* To explain **every commonly used function in Power Query**
* To help **beginners understand Power BI easily** by reading this GitHub page

---

## 🛠️ Tools Covered

* Power BI Desktop
* Power Query Editor
* GitHub (for documentation)

---

# 🔷 PART 1: POWER BI – STEP BY STEP

## 1️⃣ What is Power BI?

Power BI is a **Business Intelligence tool** used to:

* Analyze data
* Create reports and dashboards
* Convert raw data into meaningful insights

Power BI is mainly used by:

* Data Analysts
* Business Analysts
* Fresher job seekers

---

## 2️⃣ Power BI Interface Explanation

### 🔹 Home Tab

* Get Data – Import data from Excel, CSV, SQL, etc.
* Transform Data – Open Power Query Editor
* Refresh – Update data
* Publish – Upload report to Power BI Service

### 🔹 Insert Tab

* Add Text box
* Add Buttons
* Add Images
* Add Shapes

### 🔹 Modeling Tab

* Create relationships
* Manage columns
* Create measures

### 🔹 View Tab

* Page view
* Themes
* Selection pane
* Filters pane

---

## 3️⃣ Data Import (Get Data)

Steps:

1. Open Power BI Desktop
2. Click **Get Data**
3. Select data source (Excel / CSV / Folder)
4. Load or Transform data

---

## 4️⃣ Power BI Visualizations (Each Tool Explained)

### 📊 Table Chart

* Shows data in rows and columns
* Used for detailed view

### 📊 Matrix Chart

* Similar to table but supports hierarchy

### 📈 Line Chart

* Used to show trends over time

### 📊 Column Chart

* Used for comparison between categories

### 📉 Bar Chart

* Horizontal comparison

### 🎯 Scatter Plot

* Used to show relationship between two values

### 🌳 Tree Map

* Shows data using size and color

### 🎗️ Ribbon Chart

* Shows rank changes over time

### 🔻 Funnel Chart

* Shows process stages

### 🗺️ Map & Filled Map

* Used for location-based analysis

---

## 5️⃣ Filters in Power BI

### 🔹 Visual Level Filter

* Filters data for a single visual

### 🔹 Page Level Filter

* Applies to one report page

### 🔹 Report Level Filter

* Applies to entire report

---

## 6️⃣ Slicers

* Used for interactive filtering
* Types: Dropdown, List, Date slicer

---

## 7️⃣ Drill Down & Drill Through

* Drill Down – Go deeper into data
* Drill Through – Navigate to another page

---

## 8️⃣ Sorting & Formatting

* Sort ascending / descending
* Conditional formatting
* Data labels
* Tooltips

---

# 🔷 PART 2: POWER QUERY – STEP BY STEP

## 1️⃣ What is Power Query?

Power Query is used to:

* Clean data
* Transform data
* Prepare data before visualization

---

## 2️⃣ Power Query Interface

### 🔹 Home Tab

* Close & Apply
* Remove Rows
* Keep Rows
* Split Column
* Replace Values

### 🔹 Transform Tab

* Change Data Type
* Format (Upper, Lower, Trim)
* Extract

### 🔹 Add Column Tab

* Custom Column
* Conditional Column
* Index Column

---

## 3️⃣ Common Power Query Functions Explained

### 🔹 Remove Columns

Used to delete unwanted columns

### 🔹 Remove Duplicates

Used to remove repeated records

### 🔹 Split Column

Used to split text based on delimiter

### 🔹 Merge Queries

Used to join two tables

### 🔹 Append Queries

Used to combine tables vertically

### 🔹 Conditional Column

Used to apply IF condition

### 🔹 Replace Values

Used to replace wrong data

### 🔹 Change Data Type

Used to set correct data type

---

## 4️⃣ Power Query Transform Examples

* Text to Number
* Date extraction (Year, Month)
* Trim & Clean text
* Sorting data

---

## 5️⃣ Applied Steps (Very Important)

Every action in Power Query is recorded as a step.
This helps in:

* Tracking changes
* Debugging errors
* Reusing logic

---

# 🔷 PART 3: DATA ANALYSIS CONCEPTS LEARNED

## 📌 Types of Analysis

* Descriptive Analysis
* Diagnostic Analysis
* Trend Analysis
* Comparative Analysis

---

## 📌 Business Metrics

* Sales
* Profit
* Units Sold
* Discount
* Manufacturing Cost

---

# 📁 GitHub Project Structure

```
PowerBI-Learning-Notes/
│
├── Dataset/
├── PowerBI_Files/
├── Screenshots/
└── README.md
```
<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Power BI Data Visualization Assignment</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.7;
            margin: 40px;
            background-color: #f9f9f9;
            color: #333;
        }
        h1, h2, h3 {
            color: #1f4e79;
        }
        h1 {
            border-bottom: 3px solid #1f4e79;
            padding-bottom: 10px;
        }
        section {
            background: #ffffff;
            padding: 25px;
            margin-bottom: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
        }
        ul {
            margin-left: 20px;
        }
        li {
            margin-bottom: 8px;
        }
        code {
            background: #eef3f8;
            padding: 4px 6px;
            border-radius: 4px;
        }
        footer {
            text-align: center;
            margin-top: 40px;
            font-size: 14px;
            color: #555;
        }
    </style>
</head>
<body>

```
<h1>Power BI Data Visualization Assignment</h1>
<p>
    This document explains my <strong>Power BI Data Visualization Assignment</strong> using the provided financial sample data.
    The goal of this assignment is to analyze sales, profit, units sold, discounts, and time-based trends
    and present meaningful business insights through effective visualizations.
</p>

<section>
    <h2>1. Objective of the Assignment</h2>
    <p>The main objectives of this assignment are:</p>
    <ul>
        <li>To understand the structure of financial data.</li>
        <li>To analyze sales, profit, and units sold.</li>
        <li>To study the impact of discounts on profit.</li>
        <li>To identify monthly, quarterly, and yearly trends.</li>
        <li>To build interactive and meaningful dashboards using Power BI.</li>
    </ul>
</section>

<section>
    <h2>2. Dataset Description</h2>
    <p>The dataset used in this assignment is a <strong>Financial Sample Dataset</strong>. It contains the following key columns:</p>
    <ul>
        <li><strong>Country</strong> – Region where the product is sold</li>
        <li><strong>Product</strong> – Product category</li>
        <li><strong>Segment</strong> – Customer segment</li>
        <li><strong>Manufacturing Price</strong> – Cost to manufacture the product</li>
        <li><strong>Sale Price</strong> – Price at which the product is sold</li>
        <li><strong>Units Sold</strong> – Number of units sold</li>
        <li><strong>Gross Sales</strong> – Total sales before discount</li>
        <li><strong>Discount Band</strong> – Level of discount applied</li>
        <li><strong>Discounts</strong> – Discount value</li>
        <li><strong>Sales</strong> – Final sales after discount</li>
        <li><strong>Profit</strong> – Net profit earned</li>
        <li><strong>Date</strong> – Transaction date</li>
    </ul>
</section>

<section>
    <h2>3. Tools Used</h2>
    <ul>
        <li><strong>Power BI Desktop</strong> – For data modeling and visualization</li>
        <li><strong>Microsoft Excel</strong> – Source data format</li>
        <li><strong>GitHub</strong> – For version control and assignment hosting</li>
    </ul>
</section>

<section>
    <h2>4. Data Preparation (Power Query)</h2>
    <p>The following steps were performed in <strong>Power Query Editor</strong>:</p>
    <ol>
        <li>Loaded the Excel dataset into Power BI.</li>
        <li>Checked data types for all columns.</li>
        <li>Removed unnecessary or duplicate rows.</li>
        <li>Verified date format for time-based analysis.</li>
        <li>Ensured numeric columns had correct data types.</li>
    </ol>
</section>

<section>
    <h2>5. Visualizations Created</h2>

    <h3>5.1 Sales, Profit, and Units Sold Analysis</h3>
    <ul>
        <li>Clustered Column Chart to compare Sales and Profit.</li>
        <li>Line Chart to analyze Units Sold over time.</li>
        <li>Table and Matrix visuals for detailed values.</li>
    </ul>

    <h3>5.2 Time-Based Trend Analysis</h3>
    <ul>
        <li>Monthly sales and profit trend using Line Chart.</li>
        <li>Quarterly comparison using Column Chart.</li>
        <li>Yearly performance overview.</li>
    </ul>

    <h3>5.3 Discount Impact Analysis</h3>
    <ul>
        <li>Bar Chart showing Sales across Discount Bands.</li>
        <li>Profit comparison for different discount levels.</li>
        <li>Insights on how high discounts affect profit.</li>
    </ul>

    <h3>5.4 Relationship Analysis</h3>
    <ul>
        <li>Scatter Plot to analyze relationship between Manufacturing Price, Sale Price, and Profit.</li>
        <li>Outlier detection to identify unusual values.</li>
    </ul>
</section>

<section>
    <h2>6. Key Insights</h2>
    <ul>
        <li>Higher discounts increase sales volume but reduce profit margins.</li>
        <li>Products with optimized manufacturing and sale price generate higher profit.</li>
        <li>Sales and profit show seasonal trends across months and quarters
```

