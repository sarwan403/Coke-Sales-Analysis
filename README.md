# Coke-Sales-AnalysisUS Coca-Cola Sales & Profitability Analysis
🎯 Problem Framing & Objective Clarity
In a highly competitive beverage market, maximizing retail performance requires a sharp, granular understanding of geographic trends, brand affinity, and channel efficiency.

This repository presents an end-to-end data analysis project focused on answering the core business question: How can Coca-Cola optimize sales and maximize profitability across various U.S. retailers?

By dissecting key health metrics like operating profit margins and sales volume distribution, this analysis equips decision-makers with the strategic insights required to refine supply chains, optimize localized marketing, adjust regional pricing models, and strengthen key retail partnerships.

📊 Data Understanding & Preparation
The analysis is executed across two primary workbooks:

Dataset of Coke-sales-analysis-stubs.xlsx: The raw data foundation.

Coke-sales-analysis-solution.xlsx: The production-grade analytical solution featuring tiered operational tabs (Beginner, Intermediate, Advanced, Additional Analysis).

Dataset Structure
The dataset contains transaction-level details capturing retail performance across multiple vectors:

Demographics / Hierarchy: Retailer, Retailer ID, Region, State, City

Temporal: Invoice Date

Product: Beverage Brand (Coca-Cola, Diet Coke, Sprite, Fanta, Powerade, Dasani Water)

Financial Metrics: Price per Unit, Units Sold, Total Sales, Operating Profit, Operating Margin

Data Cleaning & Standardization
To ensure analytical integrity, the raw data underwent rigorous preprocessing steps:

Date Standardization: Converted varied text date formats into uniform YYYY-MM-DD features and derived a normalized Month column to support sequential time-series aggregation.

Data Type Validation: Text-formatted figures in Total Sales and Operating Profit were cleansed and converted to currency formatting ($), while ensuring Units Sold stood as integers.

Categorical Alignment: Evaluated categorical fields (Beverage Brand, Region) via distinct validation filters to ensure zero typographical duplicates or trailing spaces distorted aggregations.

Formula Verification: Recalculated and validated that Total Sales matches Price per Unit × Units Sold, and verified that Operating Margin mathematically aligned to Operating Profit ÷ Total Sales.

🔍 Exploratory Data Analysis (EDA)
Initial descriptive sweeps revealed critical systemic patterns across geographic territories and product lines:

Regional Concentration: The West Region commands the highest gross revenue market share ($2.83M+ out of $8.68M total sales), while the Midwest exhibits the lowest volume footprint, indicating an immediate market-penetration opportunity.

Temporal Scaling: Sales volumes demonstrate significant mid-year and year-end cyclical spikes, peaking dramatically during July ($1.04M) and December ($1.04M), highlighting clear seasonal beverage consumption habits.

Brand Dominance: Coca-Cola and Dasani Water serve as volume anchors, while brands like Fanta represent a significantly smaller portion of the regional revenue mix.

🛠️ Analytical Methods & Workbook Workflow
The workbook is meticulously structured to demonstrate progressive analytical depths, establishing an clean, audit-friendly pipeline:

1. Beginner Level (Beginner Tab)
Focuses on baseline macro-aggregations using core Excel functions and basic pivot tables:

Utilizes SUM and AVERAGE functions to isolate core financial metrics.

Builds high-level regional, monthly, and retailer pivot breakdowns to reveal global revenue contributors (e.g., tracking total sales distribution across entities like BevCo and Sodapop).

2. Intermediate Level (Intermediate Tab)
Introduces cross-dimensional matrix groupings to isolate product affinity by territory:

Aggregates multi-variable pivot matrices cross-referencing Month and Region against individual Beverage Brand totals.

Isolates specific product performance patterns (e.g., identifying why Coca-Cola and Dasani spike unevenly across distinct operating zones).

3. Advanced Level (Advanced Tab)
Drives structural performance indexing using advanced Excel modeling and dynamic calculations:

Implements complex lookups and multi-conditional criteria metrics (SUMIFS, AVERAGEIFS, INDEX/MATCH) to build interactive summary tables.

Provides granular views into exact operational unit flows across regional retail centers on a month-by-month basis.

4. Additional Analysis (Additional Analysis Tab)
Deepens strategic context through advanced corporate financial lenses:

Monthly Trend Analysis: Tracks Month-over-Month (MoM) revenue momentum and operating profit volatility.

Brand Contribution Mix: Evaluates each individual beverage product line by its overall % contribution to total company profit.

Margin Efficiency Ranking: Looks past raw top-line sales figures to index brands strictly by their native operational margin percentage.

💡 Strategic Insights & Actionable Recommendations
Based on the aggregated results generated across the modeling layers, the following strategic plays are outlined for Coca-Cola's regional operations:

1. Replicate West Coast Retail Frameworks Globally
Insight: The West region generates close to 33% of total revenue ($2.83M).

Action: Conduct a comparative playbook audit of West regional operations (such as pricing strategies, localized marketing spend, and product mix deployment) and port those high-velocity operational practices directly into lagging territories like the Midwest ($1.15M).

2. Capitalize on Peak Seasonality
Insight: July and December represent maximum demand windows, breaking past $1.04M in monthly sales respectively.

Action: Align supply chain logistics, prioritize warehouse inventory builds, and run high-visibility retail placement promotions immediately leading up to June and November to mitigate localized stock-outs during peak historical quarters.

3. Product Line Optimization & Margin Balancing
Insight: While Dasani Water moves high unit volumes, it commands vastly different unit pricing and profit efficiency margins compared to core carbonated flagships.

Action: Run localized price-elasticity promotions. In areas showcasing lower margins, bundle high-volume beverage products with high-margin items (Coca-Cola Classic, Diet Coke) to stabilize and increase the total basket operating margin across physical retail points.

🎨 Excel Workflow Quality & Navigation
This project adheres to professional corporate layout and dashboard guidelines:

Strict Color Consistency: Utilizes a unified color palette to structure data groups without adding unnecessary visual clutter.

Explicit Labeling Architecture: Every table, pivot field, and derived metric header is explicitly named; there are no raw unnamed columns or default Excel filler headings (Column1, Field2).

Formula Readability: Formulas are authored in clean, uppercase notation and wrap references predictably to ensure ease of external auditing.

Dynamic Structure: Aggregations utilize structured references and dynamic ranges, ensuring the underlying calculation framework scales seamlessly when refreshing or introducing subsequent quarterly transactional records.
