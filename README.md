# Personal Expense Tracker

## Overview

This project is part of my Python learning journey.

The goal is to import personal expense data from a CSV file, clean and structure the information, aggregate expenses by month and category, and generate visualizations that help analyze spending habits over time.

The project intentionally avoids advanced libraries and shortcuts whenever possible in order to understand the underlying logic behind data manipulation and time series construction.

---

## Features

* Import expense records from CSV
* Basic data cleaning and validation
* Creation of a master data model (`registros`)
* Aggregation of expenses by:

  * Year
  * Month
  * Category
* Generation of a flat table structure for analysis
* Visualization of:

  * Monthly spending by category
  * Total monthly spending
* Calculation of:

  * Monthly averages
  * Running totals
  * Month-over-month variation (MoM)

---

## Project Structure

### Raw Data

CSV file containing:

* Date
* Expense amount
* Category
* Details

### Master Model

Each CSV row is converted into a Python dictionary and stored in a list.

Example:

```python
{
    "fecha": datetime(...),
    "año": 2026,
    "mes": 6,
    "dia": 24,
    "concepto": "eat",
    "detalle": "bread",
    "gasto": 4.5
}
```

### Aggregation Layer

Expenses are grouped by:

```text
year → month → category → total expense
```

### Visualization Layer

Aggregated data is transformed into a flat structure that can be used to generate time-series charts.

---

## Learning Objectives

This project focuses on understanding:

* CSV processing
* Dictionaries and lists
* Nested loops
* Data aggregation
* Time series construction
* Basic plotting with Matplotlib
* Git and GitHub workflow

---

## Future Improvements

* Improved data validation
* Error handling
* Exporting summaries
* Additional financial metrics
* Migration to pandas for comparison purposes

---

## Author

Personal learning project by Matías Fons.
