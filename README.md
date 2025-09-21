# Month-Over-Month Analysis
**Study notes:** Month-over-month calculations across **Excel**, **MySQL**, **Python**, and **Power BI**.  
*Based on Maven Analytics Data Drill #3: Rolling Up, Looking Back*

<div align="center">
  <a href="./Calculating_Monthly_Changes.pdf">
    <img width="440" alt="image" alt="MOM" src="https://github.com/user-attachments/assets/fbc62589-7621-451a-9545-40563f68ac53" />
  </a>
  <br>
  📎 <a href="./Calculating_Monthly_Changes.pdf">Complete documentation and analysis</a>
</div>

## 🎯 Challenge
Aggregate raw coffee shop transactions by store and month, then calculate month-over-month sales changes to track business performance trends.
  <br><br>

## 📊 Dataset
Coffee shop transaction data containing 149,000 individual sales records that need to be aggregated and analyzed:
- **Raw transactions:** date, time, quantity, store_id, store_location, product details, sales amount
- **Goal:** Monthly sales by store with MoM change calculations 
  <br><br>

## 🛠️ Solutions
- **Excel:** PivotTable with "% Difference From" feature for instant MoM analysis
- **Python:** Pandas groupby with .diff() for efficient calculations  
- **MySQL:** LAG() window function in CTE for database-native processing
- **Power BI:** DAX DATEADD + CALCULATE for interactive dashboards
  <br><br>
  
## 🎯 Key Insights
| Tool | Best For | Why |
|------|----------|-----|
| **Excel** | Quick analysis | PivotTable processes 149K rows almost instantly |
| **Python** | Data processing | Pandas .diff() handles grouped calculations efficiently |
| **MySQL** | Database queries | LAG() window function keeps calculations clean |
| **Power BI** | Visual dashboards | Interactive charts with compelling visual impact |

  <br><br>
## 💡 Real-World Use Cases
Month-over-month analysis appears in retail performance tracking, seasonal trend identification, and business health monitoring across multiple locations.
  <br><br>

## 📂 Files
- [`coffee_shop_sales.csv`](https://maven-datasets.s3.us-east-1.amazonaws.com/Data+Drills/coffee_shop_sales.csv) - Raw transaction data (149,000 records)
- [`Calculating Monthly_Changes.pdf`](./Calculating_Monthly_Changes.pdf) - Complete documentation and insights
- [`Month Over Month.pbix`](./Month%20Over%20Month.pbix) - Power BI interactive dashboard
  <br><br>

## 🔗 Resources
- [Original Challenge](https://mavenanalytics.io/data-drills/rolling-up-looking-back)
- [Solution Video](https://www.youtube.com/watch?v=p77BcfCnXpc)
  <br><br>

## Connect
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="2.5%"> [Portfolio](https://atonekaboni.github.io/)
<br><img src="https://content.linkedin.com/content/dam/me/business/en-us/amp/brand-site/v2/bg/LI-Bug.svg.original.svg" width="2.5%"> [Linkedin](https://www.linkedin.com/in/tonekaboni/)
<br><img src="https://framerusercontent.com/images/1mpc8M10X3J323dCmqnRE1itRs.png" width="2%"> [Maven Portfolio](https://mavenshowcase.com/profile/9881d3c0-4031-7020-46f3-98e7d2f7790a)
