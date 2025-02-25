# Ad Campaign Lead Quality Analysis

## Overview
This project analyzes lead quality trends and the factors influencing lead performance in an advertising campaign dataset. The dataset includes approximately 3,000 leads from various sources such as Google, Yahoo, and internal campaigns. The goal is to assess lead quality, identify patterns, and provide actionable recommendations for optimizing ad spend and increasing lead conversion rates.

## Problem Statement
The key business questions addressed in this analysis are:
1. **Lead Quality Trends:** Are lead quality metrics improving or declining over time? Are these changes statistically significant?
2. **Drivers of Lead Quality:** What factors (e.g., ad placement, demographic attributes, ad type) influence lead quality rates?
3. **Optimization Opportunities:** If an advertiser increases the Cost Per Lead (CPL) by 20%, can we identify strategies to improve lead quality by 20%?

## Dataset Description
The dataset consists of 3,021 rows and 24 columns, containing the following key attributes:
- **Lead Created Date:** Timestamp of lead creation
- **Call Status:** Final outcome of each lead (Closed, EP Sent, EP Received, EP Confirmed, Unable to Contact, Invalid Profile, Doesn’t Qualify, Unknown)
- **Ad Creative & Source:** Widget name, publisher zone, partner, referral domain, landing page URL
- **Consumer Details:** Debt level, state, address score, phone score
- **Advertising Data:** Campaign name, ad group, keyword, referring keyword string

## Data Analysis Approach
### 1. Data Cleaning & Preprocessing
- Standardized categorical variables (e.g., partner names) to ensure consistency.
- Handled missing values in `AddressScore` and `PhoneScore`.
- Mapped `Call Status` into broader categories of good, bad, and neutral leads for easier analysis.

### 2. Exploratory Data Analysis (EDA)
- **Lead Quality Distribution:** Assessed the proportion of good vs. bad leads.
- **Trends Over Time:** Analyzed how lead quality changed over different time periods.
- **Impact of Ad Creative & Placement:** Evaluated the effect of different widget names, publisher zones, and referral sources on lead outcomes.
- **Consumer Segmentation:** Compared lead quality across different debt levels and states.
- **Visualization:** Used bar plots, line graphs, and heatmaps to highlight patterns and trends.

### 3. Insights & Key Findings
- Certain ad sources consistently generated higher-quality leads.
- Leads with higher address and phone scores correlated with better conversion rates.
- Some ad creatives performed better than others, indicating a need for A/B testing to refine ad formats.
- The trend analysis suggested seasonal fluctuations in lead quality.

### 4. Business Recommendations
- Focus ad spend on high-performing referral domains and publisher zones.
- Implement better lead filtering to exclude invalid profiles early in the funnel.
- Optimize ad creatives by prioritizing designs that have historically generated higher conversion rates.
- Introduce predictive modeling to forecast lead quality based on historical data.

## Technologies Used
- **Python** (Pandas, Matplotlib, Seaborn)
- **Jupyter Notebook**
- **Excel for dataset input**

## How to Run the Analysis
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/ad-campaign-analysis.git
   cd ad-campaign-analysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook Ad Campaign Lead Quality Analysis.ipynb
   ```

## Future Work
- Implement machine learning models to predict lead quality.
- Perform deeper analysis on ad creatives to refine targeting strategies.
- Explore additional external data sources for better lead scoring.

## Author
Rutuja Kokate
