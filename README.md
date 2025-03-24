# Airbnb Data Analysis and Visualization Project

## Project Overview
This project focuses on analyzing Airbnb listings data through extensive data wrangling, cleaning, and merging multiple datasets. The final goal is to create compelling, interactive Tableau visualizations that offer key business insights.

## Dataset Information
I worked with multiple Airbnb-related datasets containing information such as:
- Room types
- Prices
- Last review dates
- Neighborhood details

## Steps Followed

### 1. Data Acquisition
- Three datasets were collected:
  - `airbnb_room_type.xlsx`
  - `airbnb_price.csv`
  - `airbnb_last_review.tsv`
- Files were loaded into Jupyter Notebook using `pandas`.

### 2. Data Merging
- The datasets were merged on common keys (listing ID, host ID, etc.) using `pd.merge()`.

### 3. Data Cleaning & Wrangling
- **Handling missing values**: Missing values were replaced with appropriate placeholders or interpolated.
- **Standardizing text fields**: Room types and other categorical values were normalized to remove inconsistencies (e.g., "Entire home" vs. "entire home").
- **Date conversion**: The `last_review` column was converted to `datetime` format, and a separate `month` column was created to analyze seasonal trends.
- **Data type optimization**: Categorical and numerical variables were optimized for memory efficiency.

### 4. Exploratory Data Analysis (EDA)
- Summary statistics and visual checks using `matplotlib` and `seaborn`.
- Identified outliers and anomalies in pricing and availability.

### 5. Data Export for Visualization
- The cleaned dataset was exported as `airbnb_cleaned.csv`.

## Tableau Visualizations
Six high-impact, interactive Tableau visualizations were created, including:
1. **Price Distribution Across Neighborhoods**: A heatmap showing price variations.
2. **Room Type Distribution**: A pie chart showcasing different room types.
3. **Seasonality Trends**: A line chart analyzing bookings per month.
4. **Review Density Map**: Mapping review frequency across locations.
5. **Popular Booking Locations**: A bar chart ranking high-demand areas.
6. **Outlier Detection in Pricing**: Identifying overpriced and underpriced listings.

## Technologies Used
- **Python (Jupyter Notebook)**: `pandas`, `numpy`, `seaborn`, `matplotlib`
- **Tableau**: Interactive dashboards and charts
- **GitHub**: Version control and documentation

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/airbnb-analysis.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the Jupyter Notebook to process the data.
4. Open the Tableau workbook to explore visualizations.

## Conclusion
This project demonstrates strong data wrangling, analysis, and visualization skills. The insights derived from Airbnb data can help hosts optimize their listings and improve user experience.

---
For more details, check out the Tableau Public dashboard [https://public.tableau.com/views/AirBnBVisuals_17428070833060/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link].

