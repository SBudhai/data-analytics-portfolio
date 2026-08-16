# Global Economic Analysis

## Project Overview

This project explores global economic trends using international economic data covering 220 countries and areas from 1970 to 2021.

The analysis combines Python-based data preparation and exploratory analysis with an interactive Tableau dashboard to examine differences in economic output, GDP per capita, international trade, population, and changes in GDP across countries.

The goal of the project was to transform a large international dataset into clear and interactive visualizations that make complex economic trends easier to explore and interpret.

### View the Interactive Dashboard
(https://public.tableau.com/shared/XTYT6YK6H?:display_count=n&:origin=viz_share_link)

---

## Key Metrics

For the 2021 dashboard view:

- **$95.9 trillion** in combined GDP
- **$18.5K** average GDP per capita across countries and areas represented
- **212** countries and areas represented in 2021
- **$23.3 trillion** GDP for the largest economy

---

## Research Questions

This project explores several questions:

1. How is global economic output distributed across countries?
2. How have major economies changed between 1970 and 2021?
3. How does GDP per capita differ across countries?
4. What is the relationship between economic size, GDP per capita, population, and changes in GDP?
5. Which countries have the largest trade surpluses and deficits?
6. How can interactive visualization make international economic data easier to interpret?

---

## Tools & Technologies

- **Python** — data preparation, transformation, and analysis
- **Pandas** — data cleaning, validation, aggregation, and feature creation
- **NumPy** — numerical operations
- **Google Colab** — analysis environment
- **Tableau Public** — dashboard development and interactive visualization
- **GitHub** — project documentation and version control

---

## Dataset

The dataset contains international economic indicators covering **1970–2021**.

The original dataset contained:

- **10,512 records**
- **220 countries and areas**
- **26 original variables**

Economic indicators included:

- Gross Domestic Product (GDP)
- Gross National Income (GNI)
- GDP per capita
- Population
- Exports of goods and services
- Imports of goods and services
- Government consumption
- Household consumption
- Gross capital formation
- Manufacturing
- Agriculture
- Exchange rates

---

## Data Preparation

The dataset was prepared and analyzed using Python in Google Colab.

Data preparation included:

- Removing unnecessary whitespace from column names
- Renaming variables to improve readability
- Reviewing data types
- Checking for duplicate records
- Evaluating missing values
- Sorting observations by country and year
- Creating Tableau-friendly financial measures
- Validating country and year coverage

The dataset contained **no duplicate rows**.

Core variables, including GDP, GNI, population, and GDP per capita, contained no missing values.

Missing trade observations were retained as missing rather than replaced with zero because unavailable trade data does not necessarily indicate zero economic activity.

---

## Feature Engineering

Several additional economic indicators were created using Python.

### GDP Per Capita

GDP per capita was calculated as:

`GDP / Population`

This provides a standardized measure that allows economies of different population sizes to be compared.

### Trade Balance

Trade balance was calculated as:

`Exports - Imports`

A positive value represents a trade surplus, while a negative value represents a trade deficit.

### GDP Change

Year-over-year percentage change in current-price GDP was calculated for each country.

Because this measure is based on current-price GDP values, it is presented as **GDP Change (%)** rather than real GDP growth.

### Dashboard-Friendly Measures

Additional measures were created to simplify Tableau visualization, including:

- GDP in billions of USD
- GNI in billions of USD
- Exports in billions of USD
- Imports in billions of USD
- Trade balance in billions of USD
- Population in millions
- GDP in trillions of USD

---

## Interactive Tableau Dashboard

The Tableau dashboard provides multiple ways to explore international economic patterns.

### Dashboard Components

**Global GDP Map**

A geographic visualization displays GDP across countries for 2021, allowing users to quickly identify where global economic output is concentrated.

**GDP Trends Over Time**

A time-series visualization compares GDP trends across several major economies from 1970 to 2021.

Countries highlighted include:

- United States
- China
- Japan
- Germany
- India
- United Kingdom

**GDP vs. GDP Per Capita**

An interactive scatter plot compares countries based on GDP and GDP per capita.

Additional dimensions include:

- Bubble size representing population
- Color representing GDP change
- Country-level information available through tooltips

**Trade Balance by Country**

A diverging bar chart highlights countries with the largest trade surpluses and deficits in 2021.

**Economic KPI Cards**

The dashboard provides a high-level summary of:

- Global GDP
- Average GDP per capita
- Countries and areas represented
- Size of the largest economy

---

## Key Findings

- Combined GDP across the **212 countries and areas represented in the 2021 data was approximately $95.9 trillion**.
- The **United States was the largest economy represented in 2021**, with GDP of approximately **$23.3 trillion**.
- The time-series analysis illustrates major changes in the distribution of global economic output between 1970 and 2021, including substantial growth in China's share of global economic activity.
- GDP per capita varies considerably across countries and does not necessarily correspond directly with total economic size.
- Population, GDP, and GDP per capita provide different perspectives on economic scale and living standards, demonstrating the importance of using multiple indicators when comparing economies.
- Trade balances vary substantially across countries, with some economies recording large trade surpluses while others record significant deficits.

---

## Dashboard Interactivity

The dashboard was designed to support interactive exploration rather than provide only static visualizations.

Users can explore individual countries through geographic and chart-based visualizations and view additional economic information through tooltips.

The dashboard combines geographic, time-series, financial, and comparative visualizations to provide multiple perspectives on global economic performance.

---

## Limitations

Several limitations should be considered when interpreting the analysis:

- The dataset ends in **2021**, so the dashboard should not be interpreted as representing current economic conditions.
- GDP values are based on the measures provided in the source dataset and should not be interpreted as inflation-adjusted unless explicitly specified.
- The calculated GDP change measure uses current-price GDP and therefore represents a percentage change in nominal/current-price GDP rather than real GDP growth.
- Some observations for exports and imports are missing.
- GDP per capita and other national economic indicators provide broad economic measures but do not directly measure income distribution, inequality, quality of life, or individual household outcomes.

---

## Repository Structure

```text
global-economic-analysis/
│
├── data/
│   └── global_economy_cleaned.csv
│
├── notebooks/
│   └── global_economy_analysis.ipynb
│
├── visuals/
│   └── global_economic_dashboard.png
│
└── README.md
