# 01_cleaned_data

Place cleaned/processed datasets here.

Expected outputs from `a_Data_Preparation.ipynb`:

- `uwb_dataset_classification.csv`: Classification-ready dataset (LOS/NLOS target) in CSV format.
- `uwb_dataset_classification.parquet`: Same classification dataset in Parquet format for faster loading and smaller size.
- `uwb_dataset_regression.csv`: Regression-ready dataset with second-path range target in CSV format.
- `uwb_dataset_regression.parquet`: Same regression dataset in Parquet format for faster loading and smaller size.

CSV files in this folder are ignored by Git.
