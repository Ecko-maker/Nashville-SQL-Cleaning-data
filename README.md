# Data Analyst Portfolio Projects

A collection of data analysis, data cleaning, and visualization projects
built while practicing SQL, Python, and BI tooling. Feel free to take any
of this and make it your own — I hope it helps you land that dream job! :D

## Contents

### SQL

| File | Description |
| --- | --- |
| `COVID Portfolio Project - Data Exploration.sql` | Exploratory analysis of COVID-19 case, death, and vaccination data (joins, CTEs, temp tables, window functions, views). |
| `Tableau Portfolio Project SQL Queries.sql` | Queries used to build the companion Tableau dashboard for the COVID-19 dataset. |
| `Data Cleaning Nashville.sql` | Cleans the Nashville Housing dataset: standardizes dates, fills missing property addresses, splits address fields, normalizes categorical values, and removes duplicates. |
| `Library-Managment-system.sql` | Schema, sample data, indexes, and reporting views for a library management system (first iteration). |
| `Library_Managment_system1.sql` | Revised library management system schema with documented sections and additional analytical queries (duplicate detection, subqueries, star-schema join for BI). |

### Python

| File | Description |
| --- | --- |
| `app.py` | A [Shiny for Python](https://shiny.posit.co/py/) dashboard visualizing U.S. housing market trends (median list price, inventory, and new listings) by state and date range. |
| `SLR-Predict Salary.py` | Simple linear regression example that fits `Salary ~ YearsExperience` on `Salary_Data.csv`, plots the regression line, and predicts salary for a user-supplied years-of-experience value. |

### Notebooks

| File | Description |
| --- | --- |
| `NYC Taxi.ipynb` / `Taxi.ipynb` | Exploratory data analysis of the 2017 NYC Yellow Taxi trip dataset. |
| `Movie Portfolio Project.ipynb` | Data cleaning and exploratory analysis of a movies dataset (missing-value checks, feature engineering). |

### BI / Other

| File | Description |
| --- | --- |
| `Library_Managment PowerBI.pbix` | Power BI report built on top of the library management system data. |
| `index.html` | Standalone Leaflet map page that polls a GeoJSON feed and plots a marker's live position. |
| `campus_final.geojson` | Sample GeoJSON polygon data used for mapping experiments. |

## Getting Started

- **SQL scripts**: written against SQL Server / MySQL syntax as noted in each
  file's header comment. Point the queries at your own database/schema before
  running.
- **`app.py`**: requires the `shiny`, `shinywidgets`, `plotly`, `pandas`, and
  `faicons` packages, plus a local `state_choices.py` and the Zillow-style CSV
  extracts referenced at the top of the file.
  ```bash
  pip install shiny shinywidgets plotly pandas faicons
  shiny run app.py
  ```
- **`SLR-Predict Salary.py`**: requires `pandas`, `matplotlib`, `seaborn`, and
  `statsmodels`, plus a `Salary_Data.csv` file in the same directory.
  ```bash
  pip install pandas matplotlib seaborn statsmodels
  python "SLR-Predict Salary.py"
  ```
- **`index.html`**: open directly in a browser; it expects a
  `../data/robot_position.geojson` feed to poll for marker updates.

## License

No license specified — reuse freely for learning purposes.
