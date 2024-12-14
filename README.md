# Data Analysis Report: Cooking Sessions and User Orders

## Project Overview

### Objective
To explore how cooking session characteristics influence user orders, identify popular dishes, analyze demographic trends, and provide actionable insights for marketing and business strategies.

### Tools and Libraries
- **Python Libraries**: pandas, matplotlib, seaborn
- **Data Source**: Provided Excel file with three datasets

---

## Analysis Steps

### Step 1: Setup and Import Libraries
We installed and imported the following Python libraries:
- **pandas** for data manipulation.
- **matplotlib** and **seaborn** for visualizations.

### Step 2: Load the Datasets
The following datasets were loaded from the Excel file:
1. **User Details**
2. **Cooking Sessions**
3. **Order Details**

### Step 3: Data Cleaning
To ensure the data was clean and ready for analysis, we:
- **Handled Missing Values**:
  - Imputed numerical columns using forward or backward fill.
  - Filled missing categorical columns with the mode.
- **Ensured Data Type Consistency**:
  - Converted date fields (e.g., `Registration Date`, `Session Start`, `Order Date`) to datetime format.
- **Standardized Text**:
  - Converted categorical fields (e.g., `Favorite Meal`, `Meal Type`) to lowercase for consistency.

### Step 4: Merge Datasets
The datasets were merged into a single comprehensive dataset:
1. **Cooking Sessions** and **Order Details** were merged on `Session ID`.
2. The resulting dataset was merged with **User Details** on `User ID`.

### Step 5: Data Analysis

#### 1. Relationship Between Cooking Sessions and Orders
- **Correlation**: Calculated the correlation between average session duration and average user orders.
- **Visualization**: A scatter plot showed a positive relationship between `Duration (mins)` and `Amount (USD)`.
  
  **Key Insight**: Users with longer cooking sessions tend to place higher-value orders.

#### 2. Popular Dishes
- **Analysis**: Identified the top 3 most frequently ordered dishes.
- **Visualization**: A bar plot highlighted dish popularity.

  **Key Insight**: Certain dishes are universally popular and represent potential focus areas for promotional campaigns.

#### 3. Demographic Analysis
- **Impact of Age on Spending**: Boxplot analysis revealed spending trends by age group.
- **Regional Preferences**: A stacked bar plot highlighted variations in dish popularity by location.

  **Key Insights**:
  - Spending patterns varied significantly across age groups.
  - Certain dishes were region-specific favorites, guiding targeted marketing efforts.

### Step 6: Comprehensive Visualizations

#### Meal Preferences
- **Visualization**: A pie chart depicted the distribution of favorite meals.
- **Key Insight**: A few meal types dominate user preferences.

#### Spending by Meal Type and Duration
- **Visualization**: A heatmap showed spending patterns based on meal type and cooking session duration.
- **Key Insight**: Longer durations for specific meal types correspond to higher spending.

---

## Key Findings

### Highlights
1. **Cooking Sessions vs. Orders**:
   - Positive correlation (**0.29**) between session duration and order value.
2. **Popular Dishes**:
   - The top 3 dishes accounted for a majority of orders.
3. **Demographics**:
   - Spending trends varied across regions and age groups.
4. **Meal Preferences**:
   - A few dominant meal types drive user preferences.
5. **Spending Trends**:
   - Certain meal types and session durations are associated with higher spending.

### Recommendations
1. Focus marketing campaigns on top dishes and regional favorites.
2. Design promotions targeting specific age groups and meal types.
3. Encourage users to engage in longer cooking sessions through loyalty programs.

---

## Visualizations

Key visualizations from the analysis include:
- **Scatter Plot**: Relationship between session duration and spending.
- **Bar Plot**: Top 3 most popular dishes.
- **Boxplot**: Age vs. spending trends.
- **Stacked Bar Plot**: Regional preferences for dishes.
- **Pie Chart**: Meal preferences distribution.
- **Heatmap**: Spending by meal type and session duration.

---
