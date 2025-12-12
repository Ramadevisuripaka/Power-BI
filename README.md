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


