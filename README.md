# Data Analysis & Exploratory Data Science Portfolio

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A comprehensive collection of data analysis projects, statistical computations, and Exploratory Data Analysis (EDA) case studies. This repository demonstrates proficiency in data manipulation, statistical reasoning, and deriving actionable insights from structured datasets using the Python data analyst stack.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Analytical Methodology](#analytical-methodology)
3. [Technology Stack](#technology-stack)
4. [Repository Structure](#repository-structure)
5. [Setup & Execution](#setup--execution)
6. [Contact](#contact)

---

## Project Overview
This repository serves as a practical demonstration of end-to-end data analysis workflows. It bridges foundational algorithmic challenges (via freeCodeCamp certifications) with real-world Exploratory Data Analysis (EDA) on complex, multi-table datasets. The focus is on writing clean, vectorized code, handling missing data, and communicating findings through statistical summaries and visualizations.

---

###  Demographic Data Analyzer
* **Objective**: Parse and analyze demographic census data to answer specific statistical queries.
* **Dataset**: `adult.data.csv` (UCI Machine Learning Repository).
* **Key Analyses Performed**:
  - Count and percentage distribution of different races.
  - Average age of male vs. female demographics.
  - Percentage of individuals with a Bachelor's degree or higher.
  - Percentage of individuals with advanced degrees (Bachelors, Masters, Doctorate) who earn >50K.
  - Identification of the country with the highest percentage of >50K earners.
  - Determination of the most common occupation for individuals earning >50K in India.
* **Technical Focus**: Advanced `pandas` filtering, conditional grouping, and aggregation.

### Mean-Variance-Standard Deviation Calculator
* **Objective**: Build a robust statistical function that computes descriptive statistics for a 3x3 matrix.
* **Key Analyses Performed**: Calculates the mean, variance, standard deviation, max, min, and sum along both axes (rows and columns) and for the flattened matrix.
* **Technical Focus**: Heavy utilization of `numpy` for vectorized operations, ensuring O(1) complexity for shape validation and efficient matrix computations. Includes unit testing via `unittest` to guarantee edge-case handling (e.g., rejecting lists with fewer than 9 elements).

###  Titanic Data Analyst (EDA Notebook)
* **Objective**: Investigate the socio-economic and demographic factors that influenced survival rates during the Titanic disaster.
* **Key Analyses Performed**:
  - **Data Cleaning**: Handling missing values in `Age`, `Cabin`, and `Embarked` columns using median imputation and mode filling.
  - **Feature Engineering**: Creating new features like `FamilySize` and `Title` extracted from passenger names.
  - **Statistical Insights**: Survival rate correlation with Passenger Class (Pclass), Gender, Age groups, and Fare brackets.
  - **Visualization**: Distribution plots, survival heatmaps, and categorical bar charts using `seaborn` and `matplotlib`.

### Olist E-commerce Data Analyst (EDA Notebook)
* **Objective**: Analyze a real-world Brazilian e-commerce dataset to evaluate business performance, customer satisfaction, and logistical efficiency.
* **Dataset**: Multi-table relational data (Orders, Customers, Products, Sellers, Reviews, Geolocation).
* **Key Analyses Performed**:
  - **Data Wrangling**: Merging multiple CSV files into a unified analytical dataframe using `pandas.merge()`.
  - **Business Metrics**: Monthly order volume trends, average ticket size, and product category performance.
  - **Customer Experience**: Analysis of review scores and their correlation with delivery time (estimated vs. actual).
  - **Geospatial Insights**: State-level distribution of customers and sellers to identify regional market dominance.

---

##  Analytical Methodology
Every project in this repository follows a standardized Data Analyst pipeline:
1. **Data Ingestion**: Loading data via `pandas` with appropriate data types to optimize memory.
2. **Data Cleaning**: Identifying and resolving duplicates, handling null values, and correcting data type inconsistencies.
3. **Exploratory Data Analysis (EDA)**: Univariate and bivariate analysis to understand distributions and relationships.
4. **Statistical Validation**: Using descriptive statistics to back up visual observations.
5. **Documentation**: Inline comments and Markdown cells explaining the *why* behind each analytical step.

---

##  Technology Stack
| Category | Technologies & Libraries |
| :--- | :--- |
| **Language** | Python 3.8+ |
| **Data Manipulation** | `pandas`, `numpy` |
| **Visualization** | `matplotlib`, `seaborn` |
| **Testing** | `unittest` |
| **Environment** | Jupyter Notebook, VS Code |

---

## Repository Structure
```text
Data_Analysis/
│
├── demographic-data-analyzer/
│   ├── demographic_data_analyzer.py   # Core analysis logic
│   ├── test_module.py                 # Automated unit tests
│   └── adult.data.csv                 # Source dataset
│
├── mean-var-std-calculator/
│   ├── mean_var_std.py                # NumPy matrix computation logic
│   ├── test_module.py                 # Edge-case validation tests
│   └── main.py                        # Execution entry point
│
├── Project Notebook/
│   ├── Olist Data Analyst.ipynb       # Multi-table E-commerce EDA
│   └── Titanic Data Analyst.ipynb     # Predictive feature exploration EDA
│
├── .gitignore                         # Excludes virtual environments and large data files
├── LICENSE                            # MIT Open Source License
└── README.md                          # Comprehensive project documentation

```
##  Setup & Execution

### Prerequisites
- Python 3.8 or higher installed.
- `pip` package manager.

### Installation Steps
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Faruq871/Data_Analysis.git
   cd Data_Analysis
   ```

2. **Create and activate a virtual environment** (Best Practice):
   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows
   ```

3. **Install required dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. **Run the projects**:
   - For Jupyter Notebooks:
     ```bash
     jupyter notebook
     ```
     *Navigate to the `Project Notebook` folder and open the desired `.ipynb` file.*
   
   - For the statistical calculator tests:
     ```bash
     cd mean-var-std-calculator
     python test_module.py
     ```

---

##  Contact
I am always open to discussing data engineering, analysis techniques, or potential collaborations. 

- **GitHub**: [Faruq871](https://github.com/Faruq871)
- **LinkedIn**: [Faruq Dhiya](https://www.linkedin.com/in/faruq-dhiya/)
```
