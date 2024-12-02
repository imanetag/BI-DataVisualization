# BI-DataVisualization

# Housing Market Data Analysis - Project 1

## Project Overview

This project analyzes a housing market dataset using statistical and data visualization techniques in R. The main objective is to explore relationships among various features like crime rates, average rooms, and median home values, and to build predictive models for understanding housing prices.

## Key Features

- **Data Cleaning**:
  - Identified and handled missing values by replacing them with medians.
  - Detected and treated outliers using the IQR method.
  - Ensured data integrity by checking for duplicates.

- **Descriptive Statistics**:
  - Generated summary statistics (mean, median, mode, standard deviation).
  - Visualized distributions using histograms.

- **Correlation Analysis**:
  - Computed correlation matrices to identify relationships between variables.
  - Highlighted the strongest correlations with scatter plots.

- **Hypothesis Testing**:
  - Conducted statistical tests (e.g., t-tests, Levene's test, Shapiro-Wilk test) to assess group differences and data normality.

- **Linear Regression**:
  - Built predictive models for housing prices.
  - Evaluated models using metrics like adjusted R-squared and p-values.
  - Performed residual diagnostics to assess model validity.

- **Visualization**:
  - Created boxplots, histograms, scatter plots, and correlation heatmaps.

---

## Getting Started

### Prerequisites

Ensure you have the following software and R packages installed:

- **R** (version 4.0 or higher)
- **RStudio** (optional but recommended)
- Libraries:
  - `dplyr`
  - `ggplot2`
  - `car`
  - `reshape2`
  - `rlang`
  - `corrplot`
  - `ggcorrplot`
  - `tidyr`
  - `lmtest`
  - `e1071`

### Dataset

The dataset used in this project contains the following columns:
- `Crime.Rate`: Crime rate per capita by town.
- `Average.Rooms`: Average number of rooms per dwelling.
- `Public.Transport.Access`: Accessibility index for public transport.
- `Number.of.Schools`: Number of schools in the area.
- `Median.Home.Value`: Median value of owner-occupied homes in $1000s.

---

## Installation and Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/imanetag/BI-DataVisualization.git
   ```
2. Open the project in RStudio or your preferred R IDE.
3. Install the required R packages:
   ```R
   install.packages(c("dplyr", "ggplot2", "car", "reshape2", "rlang", "corrplot", "ggcorrplot", "tidyr", "lmtest", "e1071"))
   ```
4. Update the dataset path in the script:
   ```R
   file_path <- "./housing_data.csv"
   ```
5. Run the analysis by executing the R script.

---

## Highlights of the Analysis

1. **Missing Value Treatment**:
   - Replaced missing values in `Crime.Rate` (25 missing) and `Average.Rooms` (15 missing) with column medians.
   
2. **Outliers**:
   - Detected and replaced outliers in `Crime.Rate` and `Average.Rooms` with their respective medians.

3. **Correlation**:
   - Strong positive correlation observed between `Median.Home.Value` and `Average.Rooms` (correlation: 0.87).

4. **Linear Regression**:
   - A significant linear relationship between `Average.Rooms` and `Median.Home.Value`:
     - Coefficient: **7.046**
     - Adjusted R-squared: **0.657**
     - P-value: **< 2.2e-16**

5. **Hypothesis Testing**:
   - No significant difference in `Median.Home.Value` between high and low `Crime.Rate` groups (p-value: 0.2876).

---

Here’s a fixed and slightly enhanced version of the **Contributions** section:

---

## Contributions

We welcome contributions to this project! Here are some ways you can help:

- Improve the analysis scripts or add new functionalities.
- Provide additional datasets for analysis.
- Suggest or implement new features and visualizations.
- Fix bugs or improve code readability and documentation.

### How to Contribute

1. **Fork the Repository**:
   Click the **Fork** button at the top of this repository to create your copy.

2. **Clone Your Fork**:
   ```bash
   git clone https://github.com/yourusername/BI-DataVisualization.git
   cd BI-DataVisualization
   ```

3. **Create a Feature Branch**:
   ```bash
   git checkout -b feature-name
   ```

4. **Make Changes**:
   Edit the code, fix bugs, or add new features.

5. **Commit and Push Your Changes**:
   ```bash
   git add .
   git commit -m "Description of your changes"
   git push origin feature-name
   ```

6. **Open a Pull Request**:
   - Go to the original repository.
   - Click on the **Pull Requests** tab and create a new pull request.
   - Provide a detailed description of your changes.

