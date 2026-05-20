# Dissertation

> Python scripts for computational probability analysis and regression in spaces of empirical distributions

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/jupyter-notebook-orange.svg)](https://jupyter.org/)

---

## About

This repository contains the computational code and analysis scripts developed as part of a dissertation research project. The work focuses on regression methods in spaces of empirical distributions, with applications to demographic and mortality data analysis.

The project implements:
- Statistical modeling and probability density estimation
- Spatial-temporal analysis of mortality data (Australia, Moscow region)
- Kernel density estimation and smoothing techniques
- 3D visualization of distributional data
- Bootstrap methods and least squares regression

This code supports reproducibility of the research results and may be useful for researchers working with distributional data, demographic modeling, or nonparametric statistics.

> This project is part of ongoing academic research. Methodologies and results may be updated as the dissertation progresses.

---

## Instalation

### Prerequisites
- Python 3.9 or higher
- pip or conda package manager
- Git

### Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/Kemelbaeva/Dissertation.git
cd Dissertation
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate 
```

3. Install required packages:
```bash
pip install -r requirements.txt 
```

### Dependendencies
- Core: numpy, pandas, scipy
- Visualization: matplotlib, seaborn
- Statistics and ML: scikit-learn, statsmodels
- Interactive computing: jupyter, colab

---

## Data Structure

Dissertation/
- data/
  - .gitkeep
  - 3Dsf01.txt
  - 3Dsf01_01.txt
  - M0919h11.txt
- notebooks/
  - 3D_Australia_deaths(1921,2021,20).ipynb
  - 3D_Moscow.ipynb
  - Australia_male_mortality_distribution_3D_chart.ipynb
  - Boot_SpKernal_h1.ipynb
  - HS5-MNK-01.ipynb
  - HS5_LSM_australia_death_1921.ipynb
  - pdfIH4_smooth.ipynb
- results/
  - .gitkeep
  - figures/
- requirements.txt
- .gitignore
- SOLUTION.md

All data files are stored in plain text format. Refer to the corresponding notebooks for details on data loading and preprocessing.

> If you use external datasets, please ensure compliance with their licensing terms and cite the original sources appropriately.

---

## Notebooks Overview

| Notebook | Purpose | Key Methods | Expected Output |
|----------|---------|-------------|----------------|
| `3D_Australia_deaths(1921,2021,20).ipynb` | 3D visualization of Australian death rate distributions across ages 10-105 for years 1921-2021 (20-year intervals) | Data interpolation, 3D line plotting with matplotlib | 3D chart showing temporal evolution of age-specific death rates |
| `3D_Moscow.ipynb` | Visualization of temperature distribution dynamics in Moscow over a 13-year period | 3D plotting, density estimation, comparative visualization | 3D visualization with individual year distributions (red lines) and reference surface (blue) |
| `Australia_male_mortality_distributian_3D_chart.ipynb` | 3D visualization of male and female mortality distribution in Australia from 1921 to 2021 | Data preprocessing, 3D plotting, gender-based comparison | 3D chart comparing male (blue) and female (red) mortality rates by age and year |
| `Boot_SpKernal_h1.ipynb` | Probability density estimation using kernel methods with different kernel types | Kernel Density Estimation (KDE), Gaussian/Triangular/Spline kernels, bootstrap methods | Density estimates for temperature data saved to text files |
| `HS5-MNK-01.ipynb` | Least squares approximation of kernel density estimates using spline basis functions | Least Squares Method (LSM), Gaussian elimination, cubic spline basis functions (ph0, ph1, ph2) | Smoothed approximation curve with visualization |
| `HS5_LSM_australia_death_1921.ipynb` | Least squares approximation of Australian male mortality data for 2021 using Hermite splines | Least Squares Method (LSM), Gaussian elimination, Hermite spline basis functions | Approximated mortality curve with node points marked, saved as PNG figure |
| `pdfIH4_smooth.ipynb` | Probability density function smoothing using B-splines and least squares | Least Squares Method, B-spline basis functions (3rd order), Gaussian elimination, derivative calculations | Smoothed PDF with comparison to original function |

> Each notebook is designed to run independently. Make sure required data files are placed in the `data/` directory before execution. The notebooks demonstrate various approaches to distributional data analysis, from visualization to advanced smoothing techniques.

---

## Contact

**Author**: Kemelbaeva Aizhamal \
**Affiliation**: Siberian Federal University \
**Email**: k_aichka_r@mail.ru \
**GitHub**: [@Kemelbaeva](https://github.com/Kemelbaeva)  
