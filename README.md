# Experiment 4 - Data Wrangling and Data Visualization

## Overview
This project contains the implementation for **Experiment 4: Data Wrangling and Data Visualization** under the ECE 2112 (Advanced Computer Programming and Algorithms) course at the University of Santo Tomas. 

It demonstrates techniques for filtering tabular datasets based on categorical and numerical conditions, extracting specific feature columns, computing group summary statistics, and generating visualizations using Python's `pandas` and `matplotlib` libraries.

---

## Repository Structure

- **`board2.xlsx`**: The source ECE Board Exam dataset.
- **`ECE2112_PA4.pdf`**: Practical activity guidelines and problem specifications.
- **`Experiment_4.ipynb`**: Executable Jupyter Notebook containing all data processing steps, filtered DataFrames, statistical summary tables, and generated plots.
- **`README.md`**: Overview and execution instructions for the repository.

---

## Dataset & Features

The `board2.xlsx` dataset contains the following student attributes:
- **Categorical Features:** `Name`, `Gender`, `Track`, `Hometown`
- **Subject Scores:** `Math`, `GEAS`, `Electronics`, `Communication`
- **Calculated Metric:** `Average` (Mean score computed across all subjects)

---

## Programming Problems Covered

### A. Visayas Communication DataFrame (`VisComm`)
- **Conditions:** `Hometown == 'Visayas'` AND `Track == 'Communication'`.
- **Selected Columns:** `Name`, `Gender`, `Math`, `Electronics`, `Average`.

### B. Visayas Female DataFrame (`VisFemale`)
- **Conditions:** `Hometown == 'Visayas'` AND `Gender == 'Female'`.
- **Selected Columns:** `Name`, `Track`, `GEAS`, `Electronics`, `Average`.
- **Secondary Filtering:** Displays records where `Average >= 60` without mutating `VisFemale`.

### C. Category-Average Visualization & Analysis
- Computes mean `Average` scores grouped across `Track`, `Gender`, and `Hometown`.
- Visualizes group comparisons in a 3-panel side-by-side bar chart.
- Highlights key findings regarding sample performance across demographics.

---

## Getting Started

### Prerequisites
Make sure you have Python 3.x and the following required packages installed:

```bash
pip install pandas openpyxl matplotlib jupyter
