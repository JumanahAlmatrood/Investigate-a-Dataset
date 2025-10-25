# Investigate a Dataset (TMDb Movies Analysis)

> This project was completed as part of **Udacity’s Data Analyst Nanodegree Program**.

## Project Overview
This project is part of the Udacity Data Analyst Nanodegree. It focuses on applying the complete data analysis process on the TMDb Movies Dataset, which contains information about thousands of movies such as titles, budgets, revenues, release years, popularity, and ratings. The main goal of this project is to practice data wrangling, cleaning, exploration, visualization, and extracting meaningful insights to answer analytical questions.

## Dataset Description
The dataset used in this project is the **TMDb Movies Dataset**, which includes over 10,000 movie records.  
It contains attributes such as:
- `id`, `imdb_id`, `original_title`, `budget`, `revenue`, `runtime`, `release_year`, `vote_average`, `vote_count`, `popularity`, and `genres`.

Before analysis, the dataset required significant cleaning to handle missing data, inconsistent formatting, and invalid values such as zero budgets or revenues.

## Project Steps and Methodology

### 1. Data Wrangling
- Loaded the dataset using **Pandas**.
- Inspected the data structure, column types, and general statistics.
- Identified missing values, duplicates, and columns with invalid or irrelevant data.
- Cleaned the dataset by:
  - Removing duplicate records.
  - Dropping columns not relevant to the analysis.
  - Filtering out unrealistic data (e.g., movies with zero or negative budget/revenue).
  - Converting release dates and numeric columns to proper data types.

### 2. Exploratory Data Analysis (EDA)
After preparing the dataset, exploratory analysis was performed to answer key questions such as:
- What are the most popular genres over the years?
- How does movie budget relate to revenue?
- How have average ratings changed across years?
- What is the relationship between popularity, runtime, and success metrics?

During EDA:
- Used **grouping, aggregation, and correlation** techniques to find patterns.
- Created new columns (e.g., profit = revenue - budget) to better understand profitability.
- Applied statistical summaries to support visual insights.

### 3. Data Visualization
Visualization was an essential part of this project to clearly show patterns and trends:
- Histograms to display distributions of ratings, revenues, and runtimes.
- Scatter plots to visualize relationships between budget and revenue.
- Bar charts to compare average revenue or rating by genre and release year.
- Line plots to illustrate trends over time.

These visualizations were created using **Matplotlib** and **Seaborn** libraries and displayed within the Jupyter Notebook (`Investigate_a_Dataset.ipynb`).

### 4. Findings and Insights
From the analysis, several key insights were identified:
- There is a strong positive correlation between **budget and revenue** — higher-budget movies tend to generate higher revenues.
- Some genres such as **Action and Adventure** consistently perform well in terms of both popularity and revenue.
- The **average runtime** of successful movies tends to be between 90 and 120 minutes.
- Movie production peaked around certain years, showing clear industry trends over time.
- Movies with higher ratings are not always the most profitable, showing that popularity and profitability are distinct measures.

### 5. Limitations
- Some data points were missing or had unrealistic values.
- The dataset does not account for inflation or marketing costs, which may affect revenue interpretation.
- Genre classification was sometimes ambiguous for multi-genre films.

## Tools and Technologies
- Python  
- Jupyter Notebook  
- Pandas and NumPy for data manipulation  
- Matplotlib and Seaborn for visualization  



## Project Outcome
This project demonstrates a complete data analysis workflow, from raw dataset to cleaned, visualized insights.  
It highlights the importance of data wrangling, thoughtful questioning, and visualization in drawing meaningful conclusions from real-world data.


**Jumanah Almatrood**
