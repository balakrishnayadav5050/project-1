# project-1
# Retail Business Performance & Profitability Analysis

This project focuses on analyzing the performance and profitability of an online retail business. Using Python (Pandas, Seaborn, Matplotlib) and Tableau, the project identifies key insights and strategic recommendations to improve business operations.

## Project Overview

The dataset used contains transactional data from an online retail store. The main objectives of this project are:

1. **Data Cleaning**: Prepare the dataset for analysis by handling missing values, adding computed columns, and formatting.
2. **Profit Analysis**: Identify the most profitable products and analyze sales trends.
3. **Seasonal Trends**: Examine sales variations over time.
4. **Export Cleaned Data**: Save the cleaned dataset for further analysis in Tableau.

## Features

### Step 1: Data Loading
- Import the dataset from a CSV file.
- Display basic information and initial rows for understanding the data structure.

### Step 2: Data Cleaning
- Convert `InvoiceDate` to a datetime format.
- Create a `Total Sales` column by multiplying `Quantity` and `Price`.
- Handle missing values:
  - Fill missing `Description` values with `Unknown`.
  - Remove rows with missing `Customer ID`.

### Step 3: Profit Analysis
- Group by `Description` to calculate:
  - Total sales
  - Average price
  - Total quantity sold
- Identify the top 10 most profitable products.

### Step 4: Seasonal Trends
- Extract `Month` and `Year` from `InvoiceDate`.
- Analyze sales trends by month and visualize them using a line plot.

### Step 5: Data Export
- Save the cleaned dataset to a CSV file for use in Tableau.

### Step 6: Insights and Recommendations
- Highlight slow-moving products.
- Suggest inventory optimization strategies for high-performing months.
- Provide actionable recommendations for managing overstocked products.

## Technologies Used
- **Python Libraries**:
  - `pandas` for data manipulation
  - `seaborn` and `matplotlib` for data visualization
- **Tools**: Tableau for advanced visualization

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/retail-analysis.git
   cd retail-analysis
   ```
2. Install required Python packages:
   ```bash
   pip install pandas seaborn matplotlib
   ```
3. Place your dataset (`online_retail_.csv`) in the project directory.

## Usage

1. Run the Python script:
   ```bash
   python retail_analysis.py
   ```
2. The cleaned dataset will be exported as `cleaned_online_retail.csv`.
3. Use Tableau to visualize and further analyze the data.

## Results
- **Top 10 Profitable Products**:
  - Example: `REGENCY CAKESTAND 3 TIER`, `WHITE HANGING HEART T-LIGHT HOLDER`.
- **Seasonal Sales Trends**:
  - Clear monthly trends in total sales.

## Insights and Recommendations
1. **Slow-Moving Products**: Identify products with low sales and create strategies to boost their performance.
2. **Inventory Optimization**: Align stock levels with high-performing months to reduce wastage and increase profitability.
3. **Overstock Management**: Develop discount strategies or bundle offers for overstocked products.

# project-2
# # E-commerce Return Rate Reduction Analysis
# Ad Campaign Analysis

## Objective
Analyze ad campaign performance metrics to derive actionable insights, focusing on CTR (Click Through Rate), CPC (Cost Per Click), and demographic-based performance trends.

## Dataset Overview
The dataset contains 1,143 entries with attributes such as:
- **ad_id**: Unique ID for each ad.
- **xyz_campaign_id**: Campaign identifier.
- **fb_campaign_id**: Facebook campaign identifier.
- **age**: Target audience age group.
- **gender**: Gender of the target audience.
- **interest**: Interest category of the audience.
- **Impressions**: Number of times the ad was displayed.
- **Clicks**: Number of clicks received.
- **Spent**: Total ad spend in USD.
- **Total_Conversion**: Total number of actions taken.
- **Approved_Conversion**: Number of approved conversions.

## Tools & Technologies
- **Python**: Data cleaning, feature engineering, and visualization.
- **Libraries**: Pandas, Seaborn, Matplotlib.

## Key Features Engineered
1. **Click Through Rate (CTR)**:
   
   Formula: `CTR = Clicks / Impressions`
   
   - Measures ad effectiveness in generating clicks.

2. **Cost Per Click (CPC)**:
   
   Formula: `CPC = Spent / Clicks`
   
   - Calculates the average cost incurred per click.

## Visualizations Included
1. **Distribution of Ad Spend**:
   - Histogram showing the spend distribution across campaigns.
2. **CTR by Age Group**:
   - Boxplot comparing CTR values across different age brackets.
3. **CPC by Gender**:
   - Bar chart analyzing CPC variations by gender.

## How to Run
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/ad-campaign-analysis.git
   ```

2. **Prepare the Dataset**:
   Place the dataset in the `data/` directory.

3. **Run the Script**:
   Execute the Python script for data processing and analysis:
   ```bash
   python scripts/data_cleaning_and_analysis.py
   ```

4. **Access Outputs**:
   - Cleaned dataset: `data/cleaned_project_2.csv`
   - Visualizations: Saved in `visuals/` directory.

## Folder Structure
```
|-- README.md
|-- data/
|   |-- project_2.csv
|   |-- cleaned_project_2.csv
|-- scripts/
|   |-- data_cleaning_and_analysis.py
|-- visuals/
|   |-- ad_spend_distribution.png
|   |-- ctr_by_age_group.png
|   |-- cpc_by_gender.png
```
