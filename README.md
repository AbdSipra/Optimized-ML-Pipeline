# Optimized ML Pipeline for Binary Classification

This project benchmarks different execution strategies for a binary classification pipeline on tabular data.

The notebook compares three approaches: serial execution, parallel execution, and a hybrid setup using a local Dask backend. The goal is to measure runtime improvements while keeping model performance consistent.

## What This Project Covers

- Data preprocessing with `Pipeline` and `ColumnTransformer`
- Missing value handling
- Numeric scaling and categorical encoding
- Random Forest classification
- Runtime benchmarking across execution modes
- Accuracy, F1-score, and confusion matrix comparison
- Visualization of speed and performance trade-offs

## Execution Modes Compared

- Serial pipeline
- Parallel pipeline using `n_jobs=-1`
- Hybrid pipeline using Dask + joblib backend

## Tech Stack

- Python
- Pandas
- Scikit-learn
- Dask
- Joblib
- Matplotlib

## Files

- `optimized_ml_pipeline.ipynb` - main notebook
- `pdc_dataset_with_target (1).csv` - dataset used by the notebook

## How to Run

1. Keep the notebook and dataset file in the same repository root.
2. Install the required Python libraries used in the notebook.
3. Open `optimized_ml_pipeline.ipynb` in Jupyter Notebook or JupyterLab.
4. Run the cells in order.

## Project Goal

This repository is less about building a deployable app and more about studying how pipeline design choices affect training time and model throughput in a practical ML workflow.
