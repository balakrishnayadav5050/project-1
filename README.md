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

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue.

---

### Contact
For questions or suggestions, feel free to reach out via email: your.email@example.com.
