# Queens Public Library Network Analysis

## Project Overview

This project explores the geographic distribution and community reach of Queens Public Library locations using publicly available NYC Open Data.

The project combines Python-based data preparation and exploratory analysis with an interactive Tableau dashboard to examine the distribution of library branches across neighborhoods, ZIP codes, and community boards throughout Queens.

The goal was to transform public geographic data into an accessible visual tool that can support exploration of the library system's physical network and community coverage.

## Key Metrics

- **66** library branches
- **53** ZIP codes represented
- **14** community boards represented
- **41** neighborhoods represented

## Research Questions

1. How are Queens Public Library branches geographically distributed across Queens?
2. Which neighborhoods contain the greatest concentration of library locations?
3. How are branches distributed across community boards?
4. How can geographic visualization be used to communicate the reach of a public library network?

## Tools & Technologies

- **Python** — data preparation and exploratory analysis
- **Pandas** — data cleaning, validation, aggregation, and transformation
- **Matplotlib** — exploratory visualizations
- **Google Colab** — analysis environment
- **Tableau Public** — interactive dashboard development and geographic visualization
- **NYC Open Data** — public data source
- **GitHub** — project documentation and version control

## Data Preparation

The Queens Library Branches dataset was obtained through NYC Open Data and analyzed in Google Colab.

Initial data-quality checks included:

- Reviewing dataset dimensions and variables
- Checking for missing values
- Checking for duplicate records
- Reviewing and converting data types
- Standardizing column names
- Validating latitude and longitude fields
- Preparing geographic identifiers for analysis and visualization

The source dataset contained **66 records and 16 variables**, with **no missing values or duplicate rows**.

## Exploratory Analysis

Python was used to examine the geographic structure of the library network, including:

- Number of branches represented in the dataset
- Branch distribution across ZIP codes
- Branch distribution across community boards
- Branch distribution across neighborhoods
- Neighborhoods with the highest concentration of library locations

The cleaned dataset was then exported for visualization in Tableau Public.

## Interactive Tableau Dashboard

An interactive Tableau dashboard was developed to communicate the geographic distribution of Queens Public Library locations.

The dashboard includes:

- **KPI cards** summarizing branches, ZIP codes, community boards, and neighborhoods
- **Interactive geographic map** displaying individual library branch locations
- **Treemap** showing branch concentration by neighborhood
- **Packed bubble chart** showing branch distribution by community board
- **Interactive dashboard filtering** between geographic and categorical visualizations
- **Branch-level tooltips** providing additional geographic information

### View Interactive Dashboard

(https://public.tableau.com/shared/23ZRZ4HT2?:display_count=n&:origin=viz_share_link)

## Key Findings

- The dataset contains **66 Queens Public Library locations** distributed across **53 ZIP codes, 14 community boards, and 41 neighborhood categories**.
- Library locations are geographically distributed throughout Queens, demonstrating the broad physical reach of the library network.
- **Flushing** has the highest concentration of library locations in the neighborhood field, with **9 branches** represented in the dataset.
- **Community Board 407** has the highest number of library locations among the community boards represented, with **8 branches**.
- The distribution of locations varies across neighborhoods and community boards, which can be explored interactively through the dashboard.

## Dashboard Interactivity

Users can interact with the dashboard to explore geographic patterns in the library network.

Selecting a neighborhood in the treemap filters the other visualizations, allowing users to examine where branches associated with that neighborhood are located. Library locations on the map can also be selected to explore branch-level geographic information.

## Data Source

**NYC Open Data — Queens Library Branches**

The dataset contains branch names, addresses, geographic coordinates, ZIP codes, community boards, council districts, census tracts, and neighborhood information for Queens Public Library locations.

## Limitations

This project analyzes the **geographic distribution of library locations** rather than library performance or community demand.

The dataset does not contain measures such as circulation, program attendance, visitor counts, staffing, or service utilization. Therefore, the dashboard should be interpreted as an analysis of the library system's physical network and geographic coverage rather than a measure of service effectiveness or accessibility.

## Repository Structure

```text
queens-library-analysis/
│
├── data/
│   └── queens_library_cleaned.csv
│
├── notebooks/
│   └── queens_library_analysis.ipynb
│
├── visuals/
│   └── qpl_dashboard.png
│
└── README.md
