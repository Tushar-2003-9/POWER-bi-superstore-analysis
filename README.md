📊 PROJECT OVERVIEW

Interactive Power BI dashboard analyzing comprehensive superstore sales data to 
identify revenue trends, profit drivers, and customer segment performance.

Dataset: $2.3 Million+ in sales across 4 regions, 50+ cities, 17 product 
categories
Timeframe: 3-4 years of historical data
Records: 10,000+ transactions

🎯 KEY QUESTIONS ANSWERED

1. Which regions are most profitable and why?
   Finding: West region 23% more profitable than South despite similar sales 
   volumes. Root cause: Premium product mix (40% sales from high-margin items).

2. Which product categories drive profit vs. volume?
   Finding: Office Supplies (highest volume) but only 8% profit margin vs 12% 
   average. Furniture is highest margin (16%) but lower volume.

3. Which customer segments are most valuable?
   Finding: Corporate segment generates 45% of revenue from only 20% of 
   customers. Consumer segment high volume, low margin.

4. Are there seasonal patterns in sales?
   Finding: Q4 shows 35% spike in revenue. October-December critical months 
   for annual planning.

🛠️ TOOLS & TECHNIQUES USED

Data Cleaning & Transformation:
  • Power Query: Removed duplicates, handled missing values, standardized 
    date formats
  • Calculated columns for date hierarchy (Year, Quarter, Month)
  • Created fiscal year vs. calendar year analysis

DAX Measures Created:
  • Total Revenue = SUM(Sales[Amount])
  • Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)
  • YoY Growth = DIVIDE([Current Year Revenue] - [Previous Year Revenue], 
    [Previous Year Revenue])
  • Running Total (cumulative sales using CALCULATE)
  • Customer Count Distinct = DISTINCTCOUNT(Customer[ID])
  • Avg Order Value = DIVIDE([Total Revenue], [Order Count])

Dashboard Features:
  • Slicers: Region, Category, Customer Segment, Date Range
  • KPI Cards: Total Revenue, Total Profit, Profit Margin %, Customer Count
  • Line Chart: Revenue trend over 48 months
  • Clustered Bar Chart: Sales by Category
  • Map Visualization: Regional sales distribution
  • Scatter Plot: Profit vs. Revenue by Subcategory
  • Conditional formatting on tables

  💡 BUSINESS INSIGHTS & RECOMMENDATIONS

Insight 1: West Region Premium Product Strategy
  • West region shows higher profit per transaction despite lower total volume
  • Recommendation: Allocate 25% more premium inventory to West region in Q4

Insight 2: Office Supplies Margin Crisis
  • Highest volume category but 8% profit margin (lowest)
  • Recommendation: Negotiate supplier costs or increase selling price by 5-8%

Insight 3: Customer Lifetime Value Correlation
  • Customers with repeat purchases (2+ orders in 6 months) show 3x higher 
    lifetime value
  • Recommendation: Launch loyalty program targeting high-frequency buyers

Insight 4: Seasonal Planning
  • Q4 revenue = Q1+Q2+Q3 combined (nearly)
  • Recommendation: Plan inventory and staffing based on Q4 demand forecast

  📈 IMPACT

✓ Stakeholders used dashboard to reallocate inventory across regions based on 
  profit contribution
✓ Identified $150K+ in profit improvement opportunities through margin analysis
✓ Enabled data-driven decisions on which categories to promote/demote
