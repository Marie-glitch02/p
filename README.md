# Energy, GDP, and Scientific Contributions Data Analysis

This repository contains a data analysis project that explores energy supply, GDP, and scientific contributions across different countries. The project integrates multiple datasets to generate insights and answer key analytical questions. Below is an overview of the datasets used, the steps involved, and the key objectives of this analysis.

## Project Objectives
The primary goal of this project is to:

- Analyze and clean data related to energy supply and renewable energy indicators.
- Integrate datasets from multiple sources, including energy, GDP, and scientific rankings.
- Extract insights by answering specific questions using data manipulation techniques with Python and pandas.

## Datasets Used

### Energy Indicators
- **Source**: United Nations
- **Content**: Energy supply, energy supply per capita, and renewable energy percentage for the year 2013.

### World Bank GDP Data
- **Source**: World Bank
- **Content**: Annual GDP for countries from 1960 to 2015.

### Sciamgo Journal and Country Rank
- **Source**: Sciamgo
- **Content**: Ranking of countries based on their journal contributions in energy engineering and power technology.

## Data Preparation

### Steps Taken:

#### Energy Data Cleaning:
- Loaded data from `Energy Indicators.xls`, excluded unnecessary columns, and renamed columns for clarity.
- Converted energy supply data from petajoules to gigajoules.
- Handled missing values by replacing them with NaN.
- Removed unnecessary details such as parentheses and numbers in country names and applied specific renaming rules for consistency.

#### GDP Data Cleaning:
- Loaded data from `world_bank.csv`, skipped metadata headers, and renamed columns for readability.
- Standardized country names to align with the energy dataset.

#### Sciamgo Data Preparation:
- Loaded rankings from `scimagojr-3.xlsx` and retained the top 15 ranked countries.

#### Dataset Integration:
- Merged the three datasets using country names, keeping only common entries.
- Focused the GDP data on the last 10 years (2006-2015) for a concise analysis.
- Generated a unified dataset with 15 entries and 20 columns.

## Key Insights and Analytical Questions

### Energy and GDP Analysis:
- Explored patterns and relationships between energy supply, population, and GDP trends.

### Top Performing Countries:
- Identified the countries with the highest renewable energy percentage.
- Analyzed scientific contributions using self-citation ratios and journal rankings.

### Population Estimation:
- Estimated populations using energy supply and energy supply per capita.

### Economic Trends:
- Calculated and ranked average GDP over the last decade for the top-performing countries.
- Determined GDP changes over the analyzed period.

### Renewable Energy Insights:
- Examined trends in renewable energy production across countries.

## Tools and Libraries Used
- **Python**: Core programming language used.
- **Libraries**:
  - `pandas` for data manipulation and analysis.
  - `numpy` for numerical computations.
  - `matplotlib` and `seaborn` (optional) for visualizations.

## How to Use This Repository

### Clone the repository:
```bash
git clone https://github.com/your-repo/energy-gdp-analysis.git
```

### Install required libraries:
```bash
pip install pandas numpy
```

### Place the required data files in the `assets` folder:
- `Energy Indicators.xls`
- `world_bank.csv`
- `scimagojr-3.xlsx`

### Run the scripts in your Python environment or Jupyter Notebook.

## Future Enhancements
- Incorporate data visualization for clearer insights.
- Extend the analysis to more years and include additional countries.
- Use machine learning models to predict trends in GDP and renewable energy adoption.
