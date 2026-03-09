# Black Friday Analysis

This project analyzes consumer purchasing behavior during the Black Friday sales event using the Black Friday dataset.  
The focus is on identifying trends in customer demographics, product categories, and spending habits.  
Interactive visualizations and dashboards are provided to make the insights clear and actionable.

You can explore the interactive dashboard here:  
[Black Friday Dashboard](https://me-vikash-kumar.github.io/Black-Friday-Analysis/index.html)

## Key Highlights
- Visualizations of customer demographics such as age, gender, occupation, and city category.
- Product category analysis to identify popular and high-demand items.
- Spending trends across different customer segments.
- Interactive dashboard built with Python, Pandas, Matplotlib, and Plotly.

## Purpose
The goal of this project is to demonstrate how data analytics and visualization can be applied to retail datasets.  
It helps businesses understand customer behavior and supports better decision-making in marketing and product strategies.

## How I built this project

**Data cleaning and preprocessing**  
I inspected the raw dataset, handled missing values and duplicates, standardized categorical labels, converted types, treated outliers, and engineered features such as total purchase and age groups. All cleaning steps are documented in the analysis notebook.

**Exploratory data analysis (EDA)**  
I performed univariate, bivariate, and multivariate analyses to identify trends and customer segments. Visualizations include histograms, boxplots, heatmaps, and grouped aggregations. Key findings guided the dashboard design.

**Power BI prototype**  
I created a quick interactive prototype in Power BI to validate the layout, KPIs, and filters. This helped refine which visuals were most useful before building the final site.

**Custom HTML dashboard**  
To showcase front-end and visualization skills, I implemented a responsive HTML dashboard using JavaScript and Plotly.js. The dashboard supports linked filters, tooltips, and drilldowns. It is hosted on GitHub Pages.

**Deployment**  
The site is published at: https://me-vikash-kumar.github.io/Black-Friday-Analysis/index.html

----------------------------------------------------------------------------------------------------------------
1. Overview
I cleaned and explored the Black Friday dataset, built an initial interactive dashboard in Power BI, and then implemented a custom HTML dashboard to showcase advanced visualization and front-end skills. The final site is hosted on GitHub Pages.

2. Data cleaning and preprocessing
Goal: make the dataset analysis-ready and reliable.

Initial inspection: loaded the dataset and inspected schema, data types, and basic statistics.

Missing values: identified columns with missing values; applied context-appropriate strategies such as imputation with medians/modes, forward/backward fill for time series (if any), or flagging rows for removal when missingness was irrecoverable.

Duplicates and consistency: removed duplicate records and standardized categorical labels (e.g., city categories, product categories).

Type conversions: converted numeric-like strings to numeric types; parsed dates where present.

Outlier handling: detected extreme values using IQR and z-score methods; treated outliers by capping or investigating and removing erroneous entries.

Feature engineering: created derived features such as total purchase per transaction, customer lifetime value proxy, age groups, and product category aggregations to support richer analysis.

Encoding: encoded categorical variables for modeling or plotting (one-hot or label encoding depending on use case).

Documentation: logged cleaning steps and rationale in a notebook so the process is reproducible.

3. Exploratory data analysis (EDA)
Goal: surface patterns, anomalies, and hypotheses to test.

Univariate analysis: distribution plots for purchase amounts, counts per category, and demographic breakdowns.

Bivariate analysis: correlation analysis and cross-tabs (e.g., purchase amount by age group, gender, city category).

Multivariate analysis: pivot tables and grouped aggregations to examine interactions (e.g., occupation × product category × average spend).

Visualizations used: histograms, boxplots, bar charts, heatmaps, stacked bar charts, and scatter plots to reveal trends and segment behavior.

Key insights captured: top-selling categories, high-value customer segments, seasonal or promotional spikes (if present), and any surprising patterns worth highlighting in the dashboard.

Notebook artifacts: saved charts, summary tables, and a short narrative of findings to guide dashboard design.

4. Power BI prototype
Goal: create a quick, interactive prototype to validate insights and stakeholder flow.

Data model: imported cleaned data into Power BI; created relationships and calculated columns/measures using DAX (e.g., total sales, average order value).

Visual layout: built pages for overview KPIs, customer demographics, product performance, and time-series trends.

Interactivity: added slicers and cross-filtering so users could explore by age group, gender, city category, and product category.

Why Power BI first: rapid iteration, easy sharing with non-technical stakeholders, and quick validation of which visuals and filters were most useful.

Limitations noted: styling and custom interactions were limited compared to a hand-coded web dashboard, which motivated the HTML implementation.

5. HTML dashboard implementation (final showcase)
Goal: produce a polished, fully custom, web-hosted dashboard that demonstrates front-end and data-visualization skills.

Tech stack: HTML, CSS (Bootstrap or custom CSS), JavaScript, and visualization libraries such as Plotly.js (or D3.js for custom charts). Backend not required — data embedded as JSON or fetched from static CSV/JSON.

Architecture: modular structure with separate components for header, filters, charts, and responsive layout to work across devices.

Data pipeline in the front end: preprocessed CSV/JSON loaded via fetch; lightweight client-side transformations for filtering and aggregations to keep the site static and fast.

Interactivity implemented: linked filters, hover tooltips, drilldowns, and responsive chart resizing.

Performance optimizations: lazy loading of large datasets, aggregation on load, and minimizing DOM updates for smooth interactions.

Styling and UX: consistent color palette, clear legends and axis labels, and accessible font sizes to make insights easy to read.

Testing and cross-browser checks: validated layout and interactions in major browsers and fixed layout/JS quirks.

Deployment: published to GitHub Pages with a clean URL and ensured assets (CSS/JS) are correctly referenced for reliable hosting.

6. Challenges, learnings, and results
Challenges overcome

Handling inconsistent categorical labels and sparse missingness required careful, documented decisions.

Translating exploratory visuals into interactive, performant web charts required rethinking some aggregations for client-side performance.

Ensuring cross-browser compatibility and responsive behavior took iterative testing.

What I learned

The value of prototyping in Power BI to validate UX before investing in a custom build.

How to balance interactivity and performance in static web dashboards.

Best practices for documenting data-cleaning decisions for reproducibility.

Results

A reproducible analysis pipeline (notebook + cleaned dataset).

A Power BI prototype for quick stakeholder review.

A polished HTML dashboard hosted on GitHub Pages that demonstrates both data analysis and front-end engineering skills.


