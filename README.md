# Sales-and-Profit-BI

An interactive Tableau dashboard designed to analyze sales performance, profitability, customer behavior, product performance, and regional trends using a multi-table business dataset.

## 📊 Project Overview

This project focuses on transforming raw business data into an interactive and decision-ready Tableau dashboard.

The dataset consists of four interconnected tables:

- **Orders** — transaction-level sales, profit, quantity, discount, and order information
- **Customers** — customer details and segmentation
- **Products** — product, category, and sub-category information
- **Location** — geographic information such as city, state, region, and postal code

The tables were joined using common identifiers to create a unified dataset for analysis.

## 🎯 Objectives

- Analyze overall sales and profitability
- Identify high-performing and loss-making products
- Understand regional sales and profit distribution
- Analyze customer and segment performance
- Examine the relationship between discounts and profitability
- Build an interactive dashboard for business-oriented decision making

## 🛠️ Tools & Technologies

- **Tableau** — Data visualization & dashboard development
- **CSV** — Source datasets
- **Calculated Fields** — Profit Margin, Average Order Value, Total Orders, Total Customers, Profit per Order
- **Tableau Filters & Actions** — Interactive analysis
- **Joins** — Multi-table data integration

## 📁 Directory Structure
```text
sales-profit-intelligence-tableau/
│
├── data/
│   ├── Customers.csv
│   ├── Location.csv
│   ├── Orders.csv
│   └── Products.csv
│
├── snapshots/
│   ├── dashboard.png
|   └── data-model.png
│
└── README.md
```

## ⚡️ Data Model
The datasets were connected using the following keys:

![Data model](snapshots/data-model.png)

## 🔍 Insights
The dashboard helps identify patterns such as:

- Certain sub-categories generate significantly higher profits than others.
- Some products generate substantial sales but comparatively weak profitability.
- Loss-making sub-categories can be identified through profitability analysis.
- Geographic performance varies across regions and states.
- Discounting alone does not strongly explain profitability at the sub-category level in the current analysis.

> **Note**: The dashboard is intended for exploratory and descriptive analysis. Observed relationships should not be interpreted as causal without further statistical analysis.

---
## Dashboard
<div
  class="tableauPlaceholder"
  id="viz1787909822068"
  style="position: relative"
>
  <noscript>
    <a href="#">
      <img
        alt="Sales and Profit BI"
        src="https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Sa&#47;SalesandProfitBI&#47;SalesandProfitBI&#47;1_rss.png"
        style="border: none"
      />
    </a>
  </noscript>

  <object class="tableauViz" style="display: none;">
    <param name="host_url" value="https%3A%2F%2Fpublic.tableau.com%2F" />
    <param name="embed_code_version" value="3" />
    <param name="site_root" value="" />
    <param name="name" value="SalesandProfitBI&#47;SalesandProfitBI" />
    <param name="tabs" value="no" />
    <param name="toolbar" value="yes" />
    <param
      name="static_image"
      value="https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Sa&#47;SalesandProfitBI&#47;SalesandProfitBI&#47;1.png"
    />
    <param name="animate_transition" value="yes" />
    <param name="display_static_image" value="yes" />
    <param name="display_spinner" value="yes" />
    <param name="display_overlay" value="yes" />
    <param name="display_count" value="yes" />
    <param name="language" value="en-US" />
  </object>
</div>

<script type="text/javascript">
  var divElement = document.getElementById("viz1787909822068");
  var vizElement = divElement.getElementsByTagName("object")[0];

  if (divElement.offsetWidth > 800) {
    vizElement.style.minWidth = "420px";
    vizElement.style.maxWidth = "3000px";
    vizElement.style.width = "100%";
    vizElement.style.minHeight = "587px";
    vizElement.style.maxHeight = "3027px";
    vizElement.style.height = divElement.offsetWidth * 0.75 + "px";
  } else if (divElement.offsetWidth > 500) {
    vizElement.style.minWidth = "420px";
    vizElement.style.maxWidth = "3000px";
    vizElement.style.width = "100%";
    vizElement.style.minHeight = "587px";
    vizElement.style.maxHeight = "3027px";
    vizElement.style.height = divElement.offsetWidth * 0.75 + "px";
  } else {
    vizElement.style.width = "100%";
    vizElement.style.height = "2627px";
  }

  var scriptElement = document.createElement("script");
  scriptElement.src =
    "https://public.tableau.com/javascripts/api/viz_v1.js";

  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>


