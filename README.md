# ProgAssignment4

# ECE 2112: Experiment 4 - Data Wrangling and Data Visualization

## Overview
This project contains the implementation for **Experiment 4: Data Wrangling and Data Visualization** under the ECE 2112 (Advanced Computer Programming and Algorithms) course at the University of Santo Tomas[span_1](start_span)[span_1](end_span). 

It demonstrates techniques for filtering tabular datasets based on categorical and numerical conditions, extracting specific feature columns, computing group summary statistics, and generating visualizations using Python's `pandas` and `matplotlib` libraries[span_2](start_span)[span_2](end_span).

---

## Repository Structure

- **`board2.xlsx`**: The source ECE Board Exam dataset[span_3](start_span)[span_3](end_span).
- **`ECE2112_PA4.pdf`**: Practical activity guidelines and problem specifications[span_4](start_span)[span_4](end_span).
- **`Experiment_4.ipynb`**: Executable Jupyter Notebook containing all data processing steps, filtered DataFrames, statistical summary tables, and generated plots[span_5](start_span)[span_5](end_span).
- **`README.md`**: Overview and execution instructions for the repository.

---

## Dataset & Features

The `board2.xlsx` dataset contains the following student attributes[span_6](start_span)[span_6](end_span):
- **Categorical Features:** `Name`, `Gender`, `Track`, `Hometown`[span_7](start_span)[span_7](end_span)
- **Subject Scores:** `Math`, `GEAS`, `Electronics`, `Communication`[span_8](start_span)[span_8](end_span)
- **Calculated Metric:** `Average` (Mean score computed across all subjects)[span_9](start_span)[span_9](end_span)

---

## Programming Problems Covered

### A. Visayas Communication DataFrame (`VisComm`)
- **Conditions:** `Hometown == 'Visayas'` AND `Track == 'Communication'`[span_10](start_span)[span_10](end_span).
- **Selected Columns:** `Name`, `Gender`, `Math`, `Electronics`, `Average`[span_11](start_span)[span_11](end_span).

### B. Visayas Female DataFrame (`VisFemale`)
- **Conditions:** `Hometown == 'Visayas'` AND `Gender == 'Female'`[span_12](start_span)[span_12](end_span).
- **Selected Columns:** `Name`, `Track`, `GEAS`, `Electronics`, `Average`[span_13](start_span)[span_13](end_span).
- **Secondary Filtering:** Displays records where `Average >= 60` without mutating `VisFemale`[span_14](start_span)[span_14](end_span).

### C. Category-Average Visualization & Analysis
- Computes mean `Average` scores grouped across `Track`, `Gender`, and `Hometown`[span_15](start_span)[span_15](end_span).
- Visualizes group comparisons in a 3-panel side-by-side bar chart[span_16](start_span)[span_16](end_span).
- Highlights key findings regarding sample performance across demographics[span_17](start_span)[span_17](end_span).

---

## Getting Started

### Prerequisites
Make sure you have Python 3.x and the following required packages installed:

```bash
pip install pandas openpyxl matplotlib jupyter
