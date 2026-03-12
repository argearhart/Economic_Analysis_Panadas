# Economic Analysis with Python and FRED API

## Overview

This project explores economic data using Python, Pandas, and the FRED API. The goal is to retrieve real-world economic indicators from the Federal Reserve Economic Data (FRED) database and analyze them using data science tools.

The project demonstrates how to:

- Access economic data through an API
- Work with time series data in pandas
- Visualize trends using matplotlib and plotly
- Perform exploratory economic analysis in Jupyter notebooks

Data is sourced from the Federal Reserve Bank of St. Louis FRED database.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Plotly
- Jupyter Notebook
- fredapi
- python-dotenv

---

## Project Structure

```
Economic_Analysis_Pandas/
│
├── Economic_Analysis.ipynb
├── .env
├── .gitignore
├── requirements.txt
└── README.md
```

Notes:

- `.env` stores API credentials and is excluded from version control.
- `.venv` contains the project's virtual environment and is also ignored by Git.

---

## Setup Instructions

### 1. Clone the repository

```
git clone <repo-url>
cd Economic_Analysis_Pandas
```

---

### 2. Create a virtual environment

```
python -m venv .venv
```

Activate the environment:

Windows:

```
.venv\Scripts\activate
```

Mac / Linux:

```
source .venv/bin/activate
```

---

### 3. Install dependencies

```
pip install -r requirements.txt
```

If the requirements file is not present yet:

```
pip install pandas numpy matplotlib plotly fredapi python-dotenv
```

---

### 4. Get a FRED API Key

Create a free API key from:

https://fred.stlouisfed.org/docs/api/api_key.html

---

### 5. Store your API key securely

Create a `.env` file in the project root:

```
FRED_API_KEY=your_api_key_here
```

This file is ignored by Git to prevent exposing credentials.

---

## Running the Notebook

Start Jupyter:

```
jupyter notebook
```

Open:

```
Economic_Analysis.ipynb
```

The notebook will load the API key from the environment file and retrieve economic datasets.

---

## Example Data Sources

Common FRED series used for analysis include:

| Indicator | FRED Series |
|----------|-------------|
| Unemployment Rate | UNRATE |
| Consumer Price Index | CPIAUCSL |
| GDP | GDP |
| Federal Funds Rate | FEDFUNDS |

These datasets allow exploration of macroeconomic trends and economic cycles.

---

## Example Workflow

Typical analysis steps in the notebook:

1. Retrieve economic time series from FRED
2. Load data into pandas
3. Clean and transform the dataset
4. Create visualizations
5. Explore economic trends over time

---

## Future Improvements

Potential enhancements include:

- Comparing multiple economic indicators
- Building automated economic dashboards
- Adding forecasting models
- Expanding analysis to regional economic data

---

## License

This project is intended for educational and analytical purposes.