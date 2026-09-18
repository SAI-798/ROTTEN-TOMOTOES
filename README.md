<div align="center">
  <h1>🍅 Rotten Tomatoes Data Scraping & EDA</h1>
  <p><i>An end-to-end data pipeline from web scraping to statistical hypothesis testing.</i></p>
</div>

**Project Overview**
This repository contains a Python-based data analytics project that automates the extraction of movie data from Rotten Tomatoes and performs in-depth Exploratory Data Analysis (EDA)[cite: 9]. The complete pipeline successfully extracts, cleans, and processes 1,500 distinct movie records[cite: 7, 8].

**Tech Stack**
*   **Web Scraping:** Python, Selenium WebDriver[cite: 9]
*   **Data Manipulation:** Pandas, NumPy[cite: 7, 8]
*   **Visualization:** Matplotlib, Seaborn[cite: 3, 4]
*   **Statistical Analysis:** SciPy[cite: 1]

**Core Workflow & Features**

*   **Automated Data Extraction:** Navigates the Rotten Tomatoes interface to systematically scrape `Title`, `Year`, `Critics_Score`, `Cast`, and `Image_Link` while handling dynamic DOM elements, ultimately exporting 1,500 records to a structured DataFrame[cite: 7, 8, 9].
*   **Data Cleaning:** Addresses null values by labeling missing cast members as "Unknown" and imputing missing critic scores with the dataset's calculated median of 83.0%[cite: 6].
*   **Feature Engineering:** Segments titles into a new `Score_Category` consisting of **HIT** (>= 75%), **Average** (60-74%), and **Below Average** (< 60%)[cite: 5].
*   **Univariate & Bivariate Analysis:** Includes histograms for movie release years, pie charts detailing score distributions (revealing a 90% HIT rate), scatter plots evaluating critics' scores over time, and a ranking of top actors by average score[cite: 3, 4].
*   **Multivariate Analysis:** Features a comprehensive correlation heatmap comparing numeric variables such as `Year`, `Decade`, `Score_Numeric`, `Cast_Count`, and `Title_Length`[cite: 2].
*   **Hypothesis Testing:** Performs Chi-Square contingency testing (p-value: 0.254), which fails to reject the null hypothesis, indicating no significant statistical association between a movie's release decade and its categorical score[cite: 1, 2]. Additionally, utilizes ANOVA testing across groups, yielding an F-statistic of 2.57[cite: 1].

**Author**
*   **Sai Lakshmi Rajulapati**
*   GitHub: [Sai-A5](https://github.com/Sai-A5)
