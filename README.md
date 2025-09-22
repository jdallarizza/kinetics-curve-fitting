# kinetics-curve-fitting

This repository contains a Python script for fitting **exponential decay models** to time-course experimental data and visualizing the results.  
It uses **nonlinear regression** (`scipy.optimize.curve_fit`) to estimate parameters of a single exponential decay model and generates publication-ready plots.

It is intended to be used with jupyter notebook


## Example:
![temporal course](time_course_fitting.png)
---

## Features

- Fits time-course datasets to a **mono-exponential decay function**:  

  y = `y₀` * exp(-`k` * x)


- Reports:
  - Best-fit parameters (`y₀`, `k`)
  - Standard errors
  - Coefficient of determination (R²)

- Plots:
  - Raw data with error bars
  - Best-fit exponential decay curves
  - Multiple experimental conditions on the same figure

- Outputs a high-quality matplotlib figure (SVG export supported).

---

## Requirements

- Python 3.8+  
- Required libraries:
  - [pandas](https://pandas.pydata.org/)
  - [numpy](https://numpy.org/)
  - [matplotlib](https://matplotlib.org/)
  - [scipy](https://scipy.org/)

Install dependencies via pip:

```bash
pip install pandas numpy matplotlib scipy
