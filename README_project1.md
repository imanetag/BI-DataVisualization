
---

# 📊 Housing Market Data Analysis - Project 1

## Project Overview

This project leverages statistical methods and data visualization techniques in R to analyze a housing market dataset. By exploring relationships among features such as crime rates, average rooms, and median home values, the analysis aims to uncover insights and build predictive models for housing prices.

---

## Objectives

1. **Understand Housing Market Trends**:
   - Analyze the impact of crime rates, public transport accessibility, and average rooms on housing prices.
2. **Enhance Data Quality**:
   - Address missing values and outliers to ensure data reliability.
3. **Develop Predictive Models**:
   - Build and evaluate linear regression models to predict housing prices.
4. **Communicate Insights**:
   - Use visualizations to present key findings effectively.

---

## 🔑 Key Features

### Data Cleaning
- Addressed missing values in key variables like `Crime.Rate` and `Average.Rooms` using column medians.
- Treated outliers via the **IQR method** to maintain data consistency.
- Verified data integrity by removing duplicates.

### Statistical Analysis
1. **Descriptive Statistics**:
   - Generated key metrics such as mean, median, mode, and standard deviation.
   - Visualized distributions using histograms.
2. **Correlation Analysis**:
   - Computed correlation matrices to identify strong relationships.
   - Found a **0.87 positive correlation** between `Median.Home.Value` and `Average.Rooms`.
3. **Hypothesis Testing**:
   - Conducted t-tests, Shapiro-Wilk tests, and Levene’s tests.
   - Found no significant difference in `Median.Home.Value` between high and low `Crime.Rate` groups (p-value: 0.2876).

### Predictive Modeling
- Built **linear regression models** to predict housing prices:
  - Coefficient for `Average.Rooms`: **7.046**.
  - Adjusted R-squared: **0.657**.
  - P-value: **< 2.2e-16**, indicating a strong statistical significance.
- Performed residual diagnostics to ensure model validity.

### Data Visualization
- Created visualizations to highlight key trends:
  - **Boxplots** to identify outliers and visualize distributions.
  - **Correlation heatmaps** to present relationships.
  - **Scatter plots** for pairwise comparisons of variables.

---

## 📂 Dataset Description

The analysis is based on the following dataset with key columns:

- **`Crime.Rate`**: Crime rate per capita by town.
- **`Average.Rooms`**: Average number of rooms per dwelling.
- **`Public.Transport.Access`**: Accessibility index for public transport.
- **`Number.of.Schools`**: Number of schools in the area.
- **`Median.Home.Value`**: Median value of owner-occupied homes in $1000s.

---

## 🛠️ Getting Started

### Prerequisites

Ensure the following tools and libraries are installed:

1. **Software**:
   - **R** (version 4.0 or higher).
   - **RStudio** (optional but recommended).
2. **R Libraries**:
   ```R
   install.packages(c("dplyr", "ggplot2", "car", "reshape2", "rlang", 
   "corrplot", "ggcorrplot", "tidyr", "lmtest", "e1071"))
   ```

### Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/imanetag/BI-DataVisualization.git
   ```
2. Open the project in RStudio or your preferred IDE.
3. Update the dataset path in the script:
   ```R
   file_path <- "./housing_data.csv"
   ```
4. Run the analysis script to generate results and visualizations.

---

## 🎯 Highlights of the Analysis

### Missing Values
- Addressed 25 missing entries in `Crime.Rate` and 15 in `Average.Rooms` by imputing medians.

### Outliers
- Detected and treated outliers in `Crime.Rate` and `Average.Rooms`.

### Correlation
- Found a **strong positive correlation (0.87)** between `Median.Home.Value` and `Average.Rooms`.

### Linear Regression
- Built a statistically significant model with:
  - Coefficient of **7.046** for `Average.Rooms`.
  - Adjusted R-squared of **0.657**.
  - P-value: **< 2.2e-16**.

### Hypothesis Testing
- Found no significant relationship between `Median.Home.Value` and `Crime.Rate` categories.

---

## 📊 Sample Visualizations

1. **Correlation Heatmap**:
   - Highlights the strong relationship between `Median.Home.Value` and `Average.Rooms`.
2. **Boxplots**:
   - Displayed distributions of `Median.Home.Value` by `Crime.Rate` levels.
3. **Scatter Plots**:
   - Illustrated relationships between housing price and other variables.

---

## 🤝 Contributions

We encourage contributions to improve and expand this project. Here’s how you can help:

1. **Enhance Scripts**:
   - Refactor the code for efficiency or add new functionalities.
2. **Data Enrichment**:
   - Provide additional datasets or merge complementary data for further analysis.
3. **Visualizations**:
   - Suggest or implement new ways to present insights effectively.

### How to Contribute

1. **Fork the Repository**:
   - Use the **Fork** button on GitHub.
2. **Clone Your Fork**:
   ```bash
   git clone https://github.com/yourusername/BI-DataVisualization.git
   ```
3. **Create a New Branch**:
   ```bash
   git checkout -b feature-name
   ```
4. **Make Changes and Push**:
   ```bash
   git add .
   git commit -m "Your description of changes"
   git push origin feature-name
   ```
5. **Submit a Pull Request**:
   - Provide a detailed description of your changes.

---
