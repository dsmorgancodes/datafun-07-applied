# datafun-06-eda

## Author

Drew Morgan

## Project Overview

This project is a custom Exploratory Data Analysis (EDA) using GitHub, Git, Jupyter, pandas, Seaborn, and other popular data analytics tools. The goal is to explore, visualize, and present insights from the Titanic dataset in a clear and engaging manner.

## Dataset Description

**Name:** Titanic Dataset (Seaborn built-in)

The Titanic dataset contains demographic and travel information for 891 of the 2,224 passengers and crew aboard the RMS Titanic, which sank on April 15, 1912 after colliding with an iceberg during its maiden voyage from Southampton to New York City. The dataset is commonly used for binary classification and exploratory analysis, with the key variable being whether a passenger survived the disaster. It includes a mix of numerical features (age, fare, family size), categorical features (sex, passenger class, port of embarkation), and derived boolean indicators (adult male, traveling alone). This version is the cleaned, built-in dataset provided by the Seaborn visualization library.

**Source:** [Seaborn Titanic Dataset](https://github.com/mwaskom/seaborn-data/blob/master/titanic.csv)

**Records:** 891 rows

### Columns

| Column        | Data Type  | Description                                                        |
|---------------|------------|--------------------------------------------------------------------|
| survived      | int64      | Survival indicator (0 = No, 1 = Yes)                              |
| pclass        | int64      | Passenger class (1 = First, 2 = Second, 3 = Third)                |
| sex           | object     | Sex of the passenger (male or female)                              |
| age           | float64    | Age of the passenger in years                                      |
| sibsp         | int64      | Number of siblings/spouses aboard the Titanic                      |
| parch         | int64      | Number of parents/children aboard the Titanic                      |
| fare          | float64    | Passenger fare paid                                                |
| embarked      | object     | Port of embarkation code (C = Cherbourg, Q = Queenstown, S = Southampton) |
| class         | category   | Passenger class as a category (First, Second, Third)               |
| who           | object     | Category of passenger (man, woman, child)                          |
| adult_male    | bool       | Whether the passenger is an adult male                             |
| deck          | category   | Deck letter (A through G)                                         |
| embark_town   | object     | Port of embarkation name (Cherbourg, Queenstown, Southampton)      |
| alive         | object     | Survival status (yes or no)                                        |
| alone         | bool       | Whether the passenger was traveling alone                          |

## How to Set Up and Run This Project

### 1. Install uv (if needed)

```bash
brew install uv
```

### 2. Create Virtual Environment and Sync Dependencies

```bash
uv venv .venv
uv sync
```

### 3. Run the Notebook

```bash
uv run jupyter lab
```

Open `notebooks/dsmorgan_eda.ipynb` in VS Code or JupyterLab and run all cells from top to bottom.

## External Dependencies

- jupyterlab
- pandas
- pyarrow
- matplotlib
- seaborn
