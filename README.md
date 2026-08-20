# US Baby Names Analysis

![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-3.x-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557C?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.x-4C72B0?style=for-the-badge)
![Plotly](https://img.shields.io/badge/Plotly-6.x-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## About the Project

This project explores the development and distribution of first names in the United States based on historical birth data.

The analysis focuses on how name popularity has changed over time and which regional differences can be observed between individual US states.

The project combines exploratory data analysis, statistical evaluation and data visualization. The data is queried from a SQLite database and analyzed using Python.

Particular attention is given to the development of popular names, the comparison between the first and last recorded years, and regional differences in name popularity.

## Analysis

### Most Popular Names

The analysis identifies the most frequently given female and male names across the entire recorded period.

The total number of births associated with each name is aggregated across all available years.

### The Development of the Name Mary

The name Mary is used to examine how the popularity of an individual name changes over time.

This illustrates that a high total number of births across a long period does not necessarily mean that a name remains equally popular in more recent years.

### Regional Distribution of Seth

The regional analysis examines the distribution of the name Seth across US states.

To make states of different sizes comparable, the analysis does not rely solely on absolute birth counts. Instead, the frequency is normalized to the number of births and expressed as Seth occurrences per 10,000 births.

The results are visualized using an interactive map of the United States.

### Changes in the Most Popular Names

The three most popular names from the first and last recorded years are compared to highlight how naming trends have changed over the full observation period.

This provides a simple comparison between the beginning and the end of the dataset.

## Data Analysis

The analysis primarily uses SQL and Pandas.

SQL is used to query, filter, group and aggregate data directly from the SQLite database. Pandas is then used for further processing and analysis.

The notebooks are organized into exploration, cleaning and visualization. A separate dashboard combines the key findings of the analysis into a single interactive view.

## Dashboard

The interactive dashboard brings together the main findings of the analysis in a clear and accessible format.

It includes:

- Top 10 female names
- Top 10 male names
- Popularity of the name Mary over time
- Regional distribution of Seth across the United States
- Comparison of the top 3 names in the first and last recorded years

Plotly is used for the interactive visualizations and dashboard.

## Project Structure

```text
Names/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   ├── 01_exploration.ipynb
│   ├── 02_cleaning.ipynb
│   ├── 03_visualization.ipynb
│   └── 04_dashboard.ipynb
│
└── README.md
```

## Getting Started

```bash
# Clone the repository
git clone https://github.com/TranceMeli/Names.git

# Install dependencies
pip install pandas matplotlib seaborn plotly nbformat

# Run the notebooks in order
jupyter notebook notebooks/01_exploration.ipynb
```
