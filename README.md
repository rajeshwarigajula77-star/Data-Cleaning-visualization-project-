
# Data Cleaning & Visualization Project

## Project Overview
This project focuses on the end-to-end pipeline of handling raw, real-world data profiles—specifically identifying and rectifying data anomalies, conducting exploratory data analysis (EDA), and building analytical visualizations to communicate core data stories. 

The accompanying Python workflow automates the detection and resolution of missing entries, structural duplicates, and extreme statistical outliers before building a visual dashboard of insights.

---

## Key Features Implemented

*   **Data Deduplication:** Identified and dropped duplicate data points based on primary identification fields (`Employee_ID`), preserving the first authentic entry.
*   **Missing Value Imputation:** Implemented robust imputation strategies. Categorical missing values are filled using the dataset's **Mode**, while missing numerical fields are accurately adjusted using the dataset's **Median** to limit skewness.
*   **Outlier Management:** 
    *   Applied logical filtering boundaries to clear erroneous inputs (e.g., negative ages or values beyond human capacity).
    *   Utilized the **Interquartile Range (IQR)** filtering method to clip extreme variance anomalies in compensation profiles.
*   **Data Visualization & Reporting:** Rendered high-resolution distribution, categorical comparison, and correlation plots using `Matplotlib` and `Seaborn`.

---

## Technical Stack & Libraries
*   **Language:** Python 3.x
*   **Data Manipulation:** `pandas`, `numpy`
*   **Data Visualization:** `matplotlib`, `seaborn`
*   **File I/O:** `os`

---

## Project Structure
```text
├── data_project.py        # Complete automated Python pipeline script
├── README.md              # Project documentation and guide
└── plots/                 # Generated analytical reports (Output)
    ├── salary_distribution.png
    ├── salary_by_department.png
    └── age_vs_salary.png
