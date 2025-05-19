# 🌞 Solar Challenge Week 1

This project analyzes solar radiation datasets from three West African countries—**Benin**, **Sierra Leone**, and **Togo**—to evaluate their potential for solar photovoltaic (PV) energy development.

## 📁 Repository Structure

solar-challenge-week1/
│
├── data/ # Raw and cleaned datasets
├── notebooks/ # Jupyter notebooks for each country and comparisons
├── docs/ # Documentation files
├── dashboard_screenshots/ # Visualization outputs
├── .gitignore # Exclude virtual envs, notebooks checkpoints, etc.
├── requirements.txt # Python dependencies
└── README.md # Project overview



## 🚀 Objectives

1. **Set up a Git-based development environment** with reproducibility and CI.
2. **Perform data profiling, cleaning, and EDA** on solar radiation datasets.
3. **Compare solar potential across countries** using GHI, DNI, and DHI metrics.

---

## 🌍 Datasets Overview

Each dataset consists of ~525,600 rows (1-minute intervals for a year) and includes:
- Global Horizontal Irradiance (GHI)
- Direct Normal Irradiance (DNI)
- Diffuse Horizontal Irradiance (DHI)
- Wind Speed (WS), Gusts (WSgust), Wind Direction (WD)
- Ambient Temperature (Tamb), Module Temperatures (ModA, ModB)

---

## 📊 Key Analyses

### ✔️ Benin (Malanville)
- **Completed:** Data cleaning, EDA (diurnal/monthly patterns, wind rose, correlation).
- **Output:** `data/benin-malanville_clean.csv`
- **Notebook:** [`benin_eda.ipynb`](notebooks/benin_eda.ipynb)

### ⚠️ Sierra Leone (Bumbuna)
- **Status:** Cleaning complete; partial EDA.
- **Output:** `data/sierraleone-bumbuna_clean.csv` (pending)
- **Notebook:** [`sierra_leone_eda.ipynb`](notebooks/sierra_leone_eda.ipynb)

### ⚠️ Togo (Dapaong)
- **Status:** Cleaning complete; partial EDA.
- **Output:** `data/togo-dapaong_qc_clean.csv` (pending)
- **Notebook:** [`togo_eda.ipynb`](notebooks/togo_eda.ipynb)

---

## 📈 Planned Visualizations (Task 3)

- Boxplots comparing GHI, DNI, DHI across countries.
- Summary statistics table.
- One-way ANOVA test on GHI values.
- Bar plots for average GHI per country.

> ⚠️ Currently, Task 3 is **incomplete** due to technical issues with `matplotlib`/`seaborn` in Jupyter.

---

## 🧪 Tech Stack

- **Languages:** Python 3.x
- **Libraries:** `pandas`, `matplotlib`, `seaborn`, `scipy`, `windrose`, `jupyter`
- **Tools:** Git, GitHub Actions (CI), Jupyter Notebooks, VSCode

---

## 🔧 Setup Instructions

```bash
# Clone the repo
git clone https://github.com/Samrawitgebremaryam/solar-challenge-week1.git
cd solar-challenge-week1

# Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
