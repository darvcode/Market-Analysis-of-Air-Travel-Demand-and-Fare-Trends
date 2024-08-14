# Airline Market Analysis: Unveiling Air Travel Trends and Fare Dynamics

## Overview

In an industry as fast-moving and competitive as aviation, understanding travel patterns, fare fluctuations, and carrier performance is crucial. This project takes a deep dive into the U.S. airline market, analyzing data spanning from 1993 to 2024. The goal is to provide actionable insights on fare trends, market demand, and how airlines are positioning themselves in this ever-changing environment.

By tracking and visualizing this data, we aim to help industry professionals and interested individuals understand the market's behavior and make informed decisions.

## Dataset

- **Description:** This dataset encompasses a comprehensive view of the U.S. airline industry. It includes data points related to flight operations, fares, and market share spanning over three decades (1993-2024).
- **Source:** [US Airline Industry Dataset on Kaggle](https://www.kaggle.com/datasets/muhammadehsan000/us-airline-industry-dataset-1993-2024).

## Steps Breakdown

### 1. Data Analysis
- **Goal:** Gain a broad understanding of the dataset, examining fare trends, demand, and market share evolution.
- **Highlights:**
  - We dug into fare patterns by year and airline to identify general pricing strategies.
  - Seasonal trends in travel were explored, revealing when airlines see the highest demand.
  - We pinpointed major players in the market and tracked how their market shares changed over time.
- **Tools:** PySpark for data handling, Pandas for more refined operations, and Matplotlib/Seaborn for visualization.

### 2. Data Cleaning
- **Goal:** Prepare the dataset by addressing any inconsistencies or missing data that could affect analysis accuracy.
- **Steps:**
  - Checked for missing values and handled them by imputing missing fares with the median fare.
  - Duplicates were removed to ensure each record was unique.
  - Outliers in fare values were capped at the 99th percentile to prevent extreme values from skewing results.
  - Data was filtered to focus on the top 10 carriers by total passengers for a more concentrated analysis.
  
### 3. Feature Engineering
- **Goal:** Create new variables that provide more insight into trends and carrier performance.
- **Approach:**
  - Introduced Year-over-Year (YoY) fare changes to measure pricing strategies over time.
  - YoY passenger growth rates were calculated to monitor demand.
  - Seasonality was incorporated to distinguish between peak and off-peak travel periods.
  - Carrier delays were averaged to give a sense of how each airline is performing on punctuality.

### 4. Data Visualization
- **Goal:** Bring the numbers to life by visualizing the key trends and patterns we've uncovered.
- **Key Visuals:**
  - **Fare Trends:** Line charts that show how fares have evolved across different carriers.
  - **Market Share:** Pie charts that break down which airlines hold the most passengers during different time periods.
  - **Delays:** Bar charts that compare delays across the top airlines, sorted by popularity.
  - **Demand Patterns:** Seasonal heatmaps that highlight when air travel spikes or dips.

### 5. Market Analysis
- **Goal:** Dig into the competitive landscape and understand which airlines are dominating various routes and how fares correlate with demand.
- **Tasks:**
  - **Route Fare Comparison:** Fares were compared across carriers on similar routes to identify competitive pricing.
  - **High/Low Demand Routes:** Routes with the most and least demand were highlighted, along with which airlines are serving those routes.
  - **Market Share Over Time:** We mapped out which airlines are gaining or losing market share, looking at shifts across the years.

## Key Insights and Findings

This project has unveiled several important trends in the U.S. airline industry:
- **Pricing Fluctuations:** Fares have consistently risen over the years for certain carriers, especially during peak travel seasons, while others maintain more stable pricing.
- **Market Share Shifts:** The dominance of certain airlines has changed significantly over time, especially after 2010, showing a competitive shift in the industry.
- **Delay Patterns:** Some airlines have consistently outperformed others when it comes to punctuality, and there's a clear relationship between frequent delays and reduced passenger numbers on certain carriers.
- **Demand Dynamics:** The busiest routes aren't always the ones with the highest fares. Airlines seem to adjust pricing strategies based on both competition and passenger demand on these routes.

---

By taking a data-driven approach, this project offers a clearer picture of the U.S. airline industry's trends and can be used as a decision-making tool for stakeholders in the field. Each analysis step, from feature engineering to visualization, contributes to a richer understanding of air travel patterns over time.
