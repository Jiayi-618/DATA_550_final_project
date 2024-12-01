# DATA_550_final_project

## Project Description
This project is designed to analyze and summarize demographic and clinical data, generate visualizations, and produce a reproducible report. The workflow includes data cleaning, creating summary tables, generating scatter plots, and rendering a final report.

## Code Description

### code/00_clean_data.R
- Read raw data from the project directory.
- Save cleaned data in the `derived_data/` folder as `data_clean.rds`.

### code/01_make_table1.R
- Read cleaned data from the `derived_data/` folder.
- Generate Table 1 summarizing demographic information.
- Save Table 1 in the `table/` folder as `table_one.rds`.

### code/02_make_scatter.R
- Read cleaned data from the `derived_data/` folder.
- Generate a scatter plot showing tumor location distributions by group.
- Save the scatter plot in the `figure/` folder as `scatterplot.png`.

### code/03_render_report.R
- Render `report.Rmd` using R Markdown.
- Read data, tables, and figures from their respective locations.
- Save the compiled report in the `reports/` folder as `report.html`.

### report.Rmd
- Load cleaned data, tables, and figures from their respective locations.
- Perform descriptive analyses and display key findings, including Table 1 and scatter plots.
- Create a production-ready report for data analysis results.

---

## Synchronize Package Environment

To synchronize the package environment for this project, run the following command:

```bash
make install
