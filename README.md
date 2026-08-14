# **St. Louis Cardinals Player Performance Analysis** 

## **Project Overview**

This project evaluates St. Louis Cardinals player performance using traditional and advanced offensive metrics to support lineup and roster decision-making.

The analysis compares batting average (AVG) with on-base plus slugging (OPS) and examines whether player performance aligns with playing time. A custom metric called the **Gap** was developed to identify differences between offensive performance and lineup usage.

The project uses player statistics from the 2024 and 2025 seasons and applies Python-based data analysis to identify players who may be undervalued or overvalued based on their offensive contribution and playing time.

## **Business Question**

Which St. Louis Cardinals players may be undervalued or overvalued in lineup decisions when comparing batting average to OPS, and how can OPS provide a broader evaluation of offensive contribution relative to playing time?

Supporting questions include:

- Which players have a high OPS but relatively low playing time?
- Do players with a high batting average always provide a higher overall offensive contribution?
- Are there players who may be overvalued when using batting average instead of OPS?

## **Data Sources**

The project uses publicly available baseball statistics from:

- Major League Baseball (MLB)
- Baseball Reference

The dataset combines St. Louis Cardinals player statistics from the 2024 and 2025 seasons.

The final dataset contains **42 player observations** and includes:

- Batting Average (AVG)
- Plate Appearances (PA)
- On-Base Percentage (OBP)
- Slugging Percentage (SLG)
- On-Base Plus Slugging (OPS)
- Season

## **Data Preparation**

The 2024 and 2025 datasets were combined into a single dataset for analysis.

Python was used to:

- Load the datasets
- Prepare the data for analysis
- Convert variables to appropriate data types
- Check player information for consistency
- Check for missing values
- Generate summary statistics
- Calculate player rankings
- Create the custom Gap metric

The final dataset contained no missing values and 42 complete player observations.

## **Analysis Approach**

The project uses diagnostic analysis to examine the relationship between player performance and playing time.

**OPS** was used as the primary measure of offensive contribution, while **plate appearances (PA)** were used to represent playing time and lineup usage.

### **Gap Metric**

A custom **Gap** metric was created by comparing a player's OPS rank with their plate appearance rank.

The metric helps identify situations where offensive performance and playing time do not align.

This approach allows the analysis to identify:

- Players with strong offensive performance but limited playing time
- Players receiving greater playing time despite lower offensive performance
- Potential differences between player contribution and lineup usage

## **Key Findings**

### **OPS Provides a Broader Performance Measure**

The analysis suggests that OPS provides a broader evaluation of offensive contribution than batting average alone because it incorporates both a player's ability to reach base and generate offensive power.

### **Performance and Playing Time Do Not Always Align**

Some players demonstrated strong OPS values while receiving relatively few plate appearances.

Other players received greater playing time despite having lower OPS values.

These differences suggest that lineup usage does not always correspond directly with offensive performance.

### **Potentially Undervalued Players**

The Gap analysis identified players with strong offensive performance but relatively limited playing time.

These players may represent opportunities for teams to reconsider lineup usage and player development decisions.

### **Potentially Overvalued Players**

The analysis also identified players receiving relatively greater playing time despite lower OPS values.

This suggests that traditional playing-time decisions may not always reflect overall offensive contribution.

## **Visual Analysis**

The project includes several visual analyses to evaluate player performance and playing time, including:

- Gap metric comparisons
- Undervalued player analysis
- Overvalued player analysis
- Scatter plot comparing batting average, OPS, and playing time
- Top offensive performers based on OPS

The scatter plot uses marker size to represent plate appearances and illustrates the relationship between offensive performance and playing time.

## **Business Recommendations**

Based on the analysis, teams could:

- Incorporate OPS alongside traditional batting average when evaluating offensive performance
- Review playing-time decisions using both performance and usage data
- Identify high-performing players who may be receiving limited opportunities
- Evaluate whether players receiving significant playing time are generating sufficient offensive contribution
- Use analytics to support more objective lineup and roster decisions

## **Limitations**

The analysis focuses primarily on offensive performance and does not include other factors that may influence lineup decisions, including:

- Defensive contribution
- Injuries
- Coaching strategy
- Specific game situations

The analysis is also limited to two seasons of data.

Additionally, OPS and plate appearances operate on different scales. Because the Gap metric is based on rankings, some differences in the magnitude of player performance may be compressed.

Future improvements could include standardized metrics such as z-scores, defensive statistics, injury history, situational performance, and larger multi-season datasets.

## **Project Structure**

```text
st-louis-cardinals-player-performance-analysis/
│
├── Datasets & Python Codes/
│   ├── Data_Analysis_Marcela_Redondo.ipynb
│   ├── stl_cardinals_2024.csv
│   └── stl_cardinals_2025.csv
│
├── Report/
│   └── Final_Project_Marcela_Redondo.pdf
│
└── README.md
```
## **Programs & Tools Used**

- **Python** — data preparation, analysis, calculations, and visualization
- **Pandas** — data manipulation and analysis
- **Jupyter Notebook / Kaggle** — analytical environment
- **Microsoft Excel** — dataset organization and preparation
- **CSV** — structured data storage
- **Matplotlib** — data visualization

## **Skills Demonstrated**

- Data cleaning and preparation
- Data integration
- Exploratory data analysis
- Diagnostic analysis
- Statistical analysis
- Data visualization
- Performance analysis
- Ranking and comparative analysis
- Metric development
- Identifying performance gaps
- Translating analysis into business recommendations
- Data-driven decision-making

## **Project Context**

This project was completed as part of **CIS627: Sports Analytics** and demonstrates how data analysis can be used to support player evaluation and organizational decision-making.

The project follows an end-to-end analytical process: combining datasets, preparing and validating data, analyzing player performance, developing a custom metric, identifying patterns, and translating the findings into recommendations.

The project demonstrates skills applicable to **Data Analyst** and **Business Analyst** roles, particularly in analyzing performance data, identifying trends and gaps, and using quantitative evidence to support business decisions.
