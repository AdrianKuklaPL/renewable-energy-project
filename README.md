# Renewable Energy Project

## Objective/Goal
The primary objective of this project is to create a robust pipeline for analyzing and forecasting energy metrics to support informed decision-making in the renewable energy domain. This includes leveraging advanced algorithms and models to:

- Analyze energy demand, generation, and interchange trends.
- Develop accurate time series forecasting models to predict future energy usage.
- Visualize key metrics and trends through interactive dashboards for actionable insights.

---

## Technologies Used
This project utilizes the following technologies and tools:

- **Programming Languages**: Python 3.10+
- **Libraries**:
  - `ipywidgets`, `itertools`, `matplotlib`, `numpy`, `pandas`, `pickle`
  - `sklearn`, `sqlalchemy`, `statsmodels`, `tensorflow`, `warnings`, `xgboost`
- **Databases**:
  - MySQL on Google Cloud Platform (GCP)
- **Visualization Tools**:
  - Tableau for interactive dashboards
- **Other Tools**:
  - MySQL Workbench for SQL view creation and database management

---

## Description
This package provides a comprehensive pipeline for analyzing and forecasting energy metrics using advanced algorithms and models. The key components include:

- **Data Engineering**:
  - Retrieve data from EIA API endpoints, bypassing limitations to store datasets in JSON format.
  - Set up and manage a MySQL database on GCP, batch load data using Python scripts, and create pre-forecasting SQL views for analysis and visualization.

- **Forecasting/Modeling**:
  - Implement time series forecasting models, including SARIMA-X, XGBoost, and LSTM, with automated hyperparameter tuning.
  - Evaluate forecasts against actual demand and external benchmarks, extrapolate trends, and analyze interdependencies using PageRank algorithms.

- **Visualization**:
  - Create dashboards using Tableau to explore demand, generation, and interchange trends by balancing authority.
  - Integrate forecasted vs. actual trends and use geospatial and network data to highlight system vulnerabilities.

---

## Installation
1. Install Python 3.10 or above and an IDE like Jupyter Lab, VS Code, or PyCharm.
2. Install the required Python libraries:
   ```bash
   pip install ipywidgets itertools matplotlib numpy pandas pickle sklearn sqlalchemy statsmodels tensorflow warnings xgboost

---

## Execution
- **Data Engineering**:
  - Ensure the MySQL database is configured and populated with JSON datasets using Python scripts found in team033data_engin_code.ipynb.
  - Verify SQL views are prepared to support forecasts and visualizations. Use MySQL Workbench with the following connection specifications:
    - Connection Name: cse6242
    - Connection Method: Standard (TCP/IP)
    - Hostname: 34.23.64.152
    - Port: 3306
    - Username: readonly_user
    - Password: readonly
    - Default Schema: testing
   
- **Forecasting/Modeling**:
  - Open team033forecasting_code.ipynb.
  - Run all cells to generate fully automated forecasting outputs, including:
    - Tuned hyperparameters.
    - PageRank scores (basic and weighted) in tabular or graphical formats.

- **Visualization**:
  - Open the team033dashboard.twbx file in Tableau.
  - Use the interactive dashboard to:
    - Explore demand, generation, and PageRank analysis.
    - Filter balancing authorities and energy metrics using the dropdown menus to the right of the dashboard.

