# CIC-IDS2017 — Network Intrusion Detection

## Overview

This project aims to develop and compare machine learning models for network intrusion detection using the CIC-IDS2017 dataset.

The main objective is to analyze network traffic data, prepare relevant features, and evaluate different intrusion detection approaches.

## Project Structure

```text
projet_data/
├── data/
│   ├── raw/           # Original data (not tracked by Git)
│   └── processed/     # Processed data (not tracked by Git)
├── models/            # Trained models
├── notebooks/         # Data analysis and experiments
├── reports/           # Reports and results
├── scripts/           # Python scripts
├── nom_du_projet/     # Project Python modules
├── .gitignore
├── environment.yml
├── requirements.txt
└── README.md
```

## Work Completed

- Inspected the eight Parquet files.
- Checked dataset dimensions and column names.
- Handled infinite and missing values.
- Fixed some incorrectly encoded labels.
- Merged the data into a single unified dataset.
- Analyzed the distribution of the 15 classes.
- Investigated exact duplicates and records with identical feature values but different labels.
- Prepared the input features and target variable.
- Prepared a train-test split while accounting for identical feature vectors to prevent data leakage.

## Upcoming Work

- Train and evaluate a Random Forest model.
- Explore anomaly detection using Isolation Forest.
- Investigate an Autoencoder and potentially a Variational Autoencoder (VAE).
- Interpret model predictions using SHAP.
- Compare the performance of the different approaches.

## Dataset

The CIC-IDS2017 dataset files are not included in this GitHub repository because of their large size. They must be downloaded separately and placed in the corresponding local project directories.

The `data/raw/` and `data/processed/` directories, along with the Parquet files, are excluded from Git version control.

## Installation

Create and activate a suitable Python environment for the project, then install the required dependencies:

```bash
pip install -r requirements.txt
```

The notebooks can then be opened and executed using Jupyter Notebook or JupyterLab.

## Collaboration

This repository is intended to facilitate collaboration by sharing notebooks, scripts, documentation, and future experimental results.

Raw and processed datasets remain stored locally and are not tracked by Git.
