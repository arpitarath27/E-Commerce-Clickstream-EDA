# **E-Commerce Clickstream & Customer Behavior Analysis**

## **Project Overview**

This project explores the UCI Clickstream Data for Online Shopping to understand how users interact with an e-commerce website and identify patterns in online shopping behaviour.

The objective is to analyse browsing activity, product category preferences, page interactions and session behaviour to identify meaningful patterns that can help improve website navigation and customer engagement strategies.

## **Dataset**

* **Source:** [UCI Clickstream Data for Online Shopping](https://archive.ics.uci.edu/dataset/553/clickstream+data+for+online+shopping)  
* **Files:** `e-shop clothing 2008.csv`, `e-shop clothing 2008 data description.txt`  
* **Records:** 165,474  
* **Features:** 14

The dataset contains clickstream records from an online clothing store, including browsing sessions, product categories, product prices, page locations, countries and website page interactions.

## **Tools & Technologies**

* Python  
* Pandas  
* NumPy  
* Matplotlib  
* Seaborn  
* Google Colab

## **Data Cleaning & Preparation**

The dataset was examined for missing values, duplicate records, incorrect data types, invalid date combinations and potential outliers.

Key observations and decisions:

* No missing values or duplicate records were found.  
* Data types were appropriate for analysis.  
* Date combinations were validated, and no invalid dates were identified.  
* The IQR method flagged potential outliers in the `order` and `price` columns.  
* Potential outliers were retained because they may represent genuine browsing activity and valid product prices.

No original records were removed or modified.

## **Analysis Performed**

The project includes:

* Product category attention analysis.  
* Website page click frequency analysis.  
* Product price and browsing activity analysis.  
* Country-wise browsing activity analysis.  
* Product image location analysis.  
* Cross-category comparison of browsing behaviour.  
* Session-level browsing activity analysis.  
* Correlation analysis of session behaviour indicators.  
* Outlier detection in session activity.  
* Monthly browsing activity analysis.

Visualizations include bar charts, histograms, box plots, scatter plots, a correlation heatmap and a monthly trend chart.

## **Key Findings**

* Trousers received the highest browsing attention with **49,742 clicks**.  
* Page 1 attracted the highest activity with **93,452 clicks**.  
* Products priced at 38 USD received the highest attention with **33,883 clicks**.  
* Poland generated the highest browsing activity with **133,963 clicks**.  
* Top Left product image positions received the highest attention with **34,532 clicks**.  
* Across 24,026 sessions, users generated an average of **6.89 clicks per session**.  
* Total clicks and unique products showed a strong positive correlation of **0.97**.  
* The IQR method identified **1,962 unusual sessions** with more than 17 clicks.  
* April recorded the highest monthly browsing activity, while August recorded the lowest.

## **Business Recommendations**

* Improve product placement and give greater visibility to popular product categories.  
* Optimize website navigation to make important products accessible from the initial pages.  
* Analyse product-level browsing patterns before making pricing or promotional decisions.  
* Focus on major customer regions, particularly Poland, when planning website improvements.  
* Explore ways to encourage users to discover more products and navigate through additional pages.  
* Monitor monthly browsing trends to identify changes in website engagement.

## **Limitations**

* The dataset contains clickstream records from 2008, so the observed patterns may not represent current online shopping behaviour.  
* The dataset records browsing activity but does not contain confirmed purchase records or an explicit conversion variable.  
* Click frequency does not necessarily indicate customer interest, purchase intention or actual sales.  
* Some categorical variables contain coded values that require reference mappings for interpretation.  
* Monthly activity is based on total clicks, and differences in observation periods or sample sizes may affect comparisons.  
* The analysis identifies associations and browsing patterns, not causal relationships.

## **Project Structure**

```
Project Structure
Online Shopping Clickstream EDA/
│
├── data/
│   └── raw/
│       ├── e-shop clothing 2008.csv
│       └── e-shop clothing 2008 data description.txt
│
├── notebooks/
│   └── Online_Shopping_Clickstream_EDA.ipynb
│
├── reports/
│   └── E-Commerce_Clickstream_Report.pdf
│
├── presentation/
│   └── E-Commerce_Clickstream_EDA_Presentation.pptx
│
└── README.md
```

## **Conclusion**

This exploratory analysis identifies meaningful patterns in online shopping activity, including product category preferences, website page interactions, geographical activity and session engagement. The findings highlight opportunities to improve website layout, product visibility and user engagement strategies. However, actual purchasing behaviour and customer conversion cannot be evaluated using this dataset because confirmed purchase records are not available.

&nbsp;