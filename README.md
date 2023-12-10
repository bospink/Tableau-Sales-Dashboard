# Tableau Sales Dashboard

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)

### Project Overview
---

I created a visually appealing, informative and interactive dashboard in **Tableau** that showcases important insights into sales performance of an online store for US market by using Tableau's advanced data visualization and filtering features.


### Data Sources

Sales Data: I got csv files from *Etsy Download Shop Data*, the *"Order Item"* CSV for each year (report of shop sales at an individual item level). Then I combined those CSV files into one Excel workbook named "PinkBau2015_2023", containing detailed information about each sale made by the store.

### Tools

- **Excel** - Data Cleaning
- **Tableau** -Data Analysis - Data Visualization

### Data Cleaning

I cleaned and formatted the data in Excel, which I explained in detail in my [Excel Project](https://github.com/bospink/Excel_project).

### Exploratory Data Analysis

This is the step where I needed to think about the design of the dashboard and what Sheets to create.

EDA involved exploring the sales data to answer key questions, such as:

- Which states sales best?
- What is the total revenue for each year?
- Which products are top sellers?
- What is the best selling month by year?

I started with connecting the data source - Exel workbook "PinkBau2015_2023", containing detailed information about each sale made by the store.

Then I proceed with making the Sheet1 using **maps** filtered by `US State`, with Marks *Color* set up as `US State` and *Size* as `CNT(EtsySoldItems)`.

Sheet2 is intended for Total Revenue by Year filtered by `Country: United States`, which I have presented as a **bar chart**.

For Top Selling Products I chose **packed bubbles** chart filtered by `Country: United States` and `Year`. Marks *Size* is `SUM(Quantity)`, while *Label* and *Color* are `Product`.

Finnaly, the Sheet4 rapresents the best selling month using **treemaps**, with Marks *Color* and *Size* as `SUM(Quantity)` and *Label*s `Month` and `SUM(Quantity)`.


Now it's time to create the **Dashboard**.

In the upper part I will place the logo and title (explanation about the report). 

I started dragging the sheets as floating objects and placing them in the proportions that seemed best for effective visualization. 

I changed the background color and opacity to match the store logo. Then I went to `Format Menu > Shading… > Format` each view's worksheet by shading with color *None* (for better UI design, layering of graphs over pictures).

There's still work left to add interactive relationship between dashboard objects (filter to multiple worksheets) by going to `Dashboard > Actions > Edit Filter Action`. I inserted `Year` for the filter on all sheets. 

My interactive Dashboard in Tableau is complete.

![Store_Sale_Dashboard_Tableau](https://github.com/bospink/Tableau-Sales-Dashboard/assets/126882792/332b6a1d-83e3-431d-81ea-9e50d195234b)


### Findings
---
The anlaysis results are summarized as follows:

1. The store sales have been steadily increasing over the past years reaching a noticable peak during 2022. Then there would be a slight drop caused by the change in the taxation for the store in 2023 and thus the increase in product prices.

2. Product Category *Litter Box Cabinet* is the best-performing category in terms of sales and revenue.

3. The best period for sales is at the end of the year, which is expected due to the holidays.

### Recommendations
---
- Invest in marketing and brand promotion which will lead to an increase in demand for the product and thus the level of sales will be maintained.
- Focus on expanding and promoting products in *Litter Box Cabinet* category.
- Encourage the purchase of products in the first months of the year with a help of coupons and weekly discounts.
