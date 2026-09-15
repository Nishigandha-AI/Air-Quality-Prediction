# Beijing PM2.5 Air Quality Prediction

## Overview

This project predicts **hourly PM2.5 concentration** using air-quality and meteorological data collected from multiple monitoring stations in Beijing.

The workflow includes data preprocessing, feature engineering, model training, evaluation, and SHAP-based model interpretation. Multiple regression models are compared, with **XGBoost** used as the final model.

## Dependencies

The project was developed and tested with the following versions:

```text
Python        3.13.5
pandas        2.2.3
numpy         2.3.5
matplotlib    3.10.8
seaborn       0.13.2
scikit-learn  1.8.0
xgboost       3.1.3
shap          0.50.0
```

Install the required dependencies:

```bash
pip install pandas==2.2.3 numpy==2.3.5 matplotlib==3.10.8 seaborn==0.13.2 scikit-learn==1.8.0 xgboost==3.1.3 shap==0.50.0
```

Or:

```bash
pip install -r requirements.txt
```

## Execution Steps

### 1. Clone the repository

```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Download the dataset

Download the **Beijing Multi-Site Air-Quality Data** dataset and place it in the project directory.

### 4. Update the dataset path

Open the notebook and update the dataset path to your local file location if required.

### 5. Run the notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Beijing_AirQuality_Assessment_V2.ipynb
```

Run all cells **from top to bottom**.

The notebook performs:

**Data Loading → Cleaning → Feature Engineering → Model Training → Evaluation → SHAP Analysis**

## Dataset

* **Dataset:** Beijing Multi-Site Air-Quality Data
* **Period:** 2013–2017
* **Frequency:** Hourly
* **Stations:** 12
* **Prediction Target:** PM2.5 (`µg/m³`)

## Models

The following models are evaluated:

* Linear Regression
* Ridge Regression
* Random Forest
* XGBoost

Models are evaluated using **MAE, RMSE, and R²**.

## Project Structure

```text
Beijing-PM2.5-Prediction/
│
├── Beijing_AirQuality_Assessment_V2.ipynb
├── requirements.txt
├── README.md
├── Technical_Report.pdf
└── data/
    └── dataset.zip
```

## Documentation

For detailed methodology, analysis, model results, and conclusions, refer to the **Technical Report**.
