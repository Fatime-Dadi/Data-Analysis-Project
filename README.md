# Uber Fares Dataset Analysis

This project performs advanced exploratory data analysis (EDA), data cleaning, and feature engineering on an Uber fares dataset for the course "Introduction to Big Data Analytics INSY 8413". The cleaned and enhanced datasets are suitable for further analysis and Power BI dashboard development.

## Project Structure

```
data/
    uber.csv                # Raw Uber fares dataset
notebooks/
    cleaning_notebook.ipynb # Main analysis and cleaning notebook
powerBI/
    uber_analysis.pbix      # Power BI dashboard (not included here)
report/
    final_report.md         # Final report
```

## Getting Started

### 1. Clone the Repository

Clone this repository to your local machine and navigate to the project directory.

### 2. Install Required Packages

Install the necessary Python packages using pip:

```sh
pip install pandas numpy matplotlib seaborn scipy scikit-learn plotly geopy folium
```

### 3. Data Preparation

- Place the raw dataset (`uber.csv`) in the `data/` directory.

### 4. Run the Notebook

Open `notebooks/cleaning_notebook.ipynb` in Jupyter Notebook or VS Code and run all cells sequentially.

The notebook performs the following steps:

#### a. Data Loading & Initial Exploration

- Loads the raw Uber fares data.
- Displays dataset structure, data types, and missing values.

#### b. Data Quality Checks

- Checks for duplicates, missing values, and outliers.
- Analyzes fare amounts, passenger counts, and datetime validity.

#### c. Data Cleaning

- Removes duplicate records.
- Filters out invalid fare amounts (negative, zero, extreme values).
- Removes invalid passenger counts and geographic coordinates.
- Drops rows with any remaining null values.

#### d. Feature Engineering

- Extracts datetime features (hour, day, month, etc.).
- Categorizes time of day and peak hours.
- Calculates trip distances (Haversine and Manhattan).
- Computes economic features (fare per mile, per passenger, etc.).
- Categorizes fares and trip distances.
- Adds geographic features (distance to landmarks, borough identification).
- Adds seasonal and holiday indicators.

#### e. Output

- Saves the cleaned dataset as `data/uber_cleaned.csv`.
- Saves the enhanced dataset with engineered features as `data/uber_enhanced.csv`.

### 5. Next Steps

- Use the cleaned/enhanced datasets for further analysis or visualization (e.g., in Power BI).
- Refer to `report/final_report.md` for insights and findings.

## Notes

- The notebook is designed for reproducibility; ensure all dependencies are installed.
- The cleaning and feature engineering steps are tailored for NYC Uber data and may need adjustment for other datasets.

---

**Author:**  
Fatime Dadi Wardougou(25858)
INSY 8413 -
