# CDS 2413 – COVID-19 Recovery Data Analysis

Group project for CDS 2413. We analyse a COVID-19 patient dataset (70,000 records) and model
`days_to_recovery`, the number of days a patient takes to recover.

## Repository structure

```
CDS2413-COVID19-Recovery-Analysis/
├── README.md               project overview (this file)
├── requirements.txt        Python packages needed to run the notebooks
├── .gitignore              files Git should not track
├── notebooks/
│   ├── covid.csv           dataset (COVID-19 Recovery Dataset, Kaggle)
│   ├── D1.ipynb            D1: sampling, descriptive statistics, charts, hypothesis tests
│   ├── D2.ipynb            D2: preprocessing, regression, classification, clustering
│   └── figures/            charts saved by D2.ipynb
└── reports/
    ├── D1_Data_Analysis_Report_MahraMira.docx   Deliverable 1 (CLO1, CLO2)
    ├── D2_ML_Report_MahraMira.docx              Deliverable 2 (CLO3)
    └── D3_Data_Versioning_Report.docx           Deliverable 3 (CLO4)
```

## How to run

```
pip install -r requirements.txt
cd notebooks
jupyter notebook
```

Open `D1.ipynb` or `D2.ipynb` and run all cells. Both notebooks read `covid.csv` from the
`notebooks` folder and use `random_state = 42`, so the results are reproducible.
## Team members

- Mahra
## Key results
- Regression: best model Lasso, R2 close to 0 (no predictive signal).
- Classification: best model SVM, macro F1 = 0.498 (close to chance).
- Clustering: K-means with k = 4 (silhouette 0.406).

