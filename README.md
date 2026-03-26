# CSC3105 Project

## File Mapping to Assignment Components

Our files are organized to match the assignment questions and implementation flow:

- `a_Data_Preparation.ipynb` → **(a) Data Preparation/Preprocessing**
- `b_Data_Mining_Classification.ipynb` → **(b) Data Mining (Classification)**
- `b_Data_Mining_Regression.ipynb` → **(b) Data Mining (Regression)**
- `c_Data_Visualization.ipynb` → **(c) Data Visualization** (consolidated visualizations)
- `d_Result_Analysis.ipynb` → **(d) Result Analysis**

Data visualization is performed throughout the project, while consolidated plots can be found in `c_Data_Visualization.ipynb`.

## ML Scope

- Supervised learning: classification or regression
- Unsupervised learning: clustering

The project focuses on:

1. **Prediction of LOS/NLOS classifier for two dominant shortest paths**
   - If the first path is LOS, the next path is NLOS.
   - If the first path is NLOS, the next path is NLOS.
   - LOS is always the shortest path if it exists.

2. **Distance estimator for two dominant shortest paths**
   - Use `FP_IDX` and measured range to correlate to the next second dominant path where possible.

## Required Implementation Considerations

### (a) Data Preparation/Preprocessing

1. Decide whether data reduction is needed.
2. Decide whether feature extraction or transformation is needed.
3. Decide whether class labeling is needed for two-path classification and estimation.
4. Decide the need for data cleaning.
5. Perform feature importance ranking.
6. Decide whether synthetic data is needed for robustness.

### (b) Data Mining

1. Decide between supervised vs unsupervised learning and select preferred algorithms.
2. Decide train/test split ratio (e.g., 70:30 or 80:20).
3. Evaluate performance using suitable metrics (e.g., RMSE, confusion matrix, ROC).

### (c) Data Visualization

1. Plot relevant performance indicators to support choices and results from parts (a) and (b).

### (d) Result Analysis

1. Justify results with theoretical understanding.

## Repository Notes

- Input data is stored under `Input_Data/`.
- Trained model outputs are stored under `Output_Models/`.
- Large data/model artifacts are ignored via `.gitignore`, while folder structure is preserved with placeholder README files.
- For notebook output cleaning setup, see `SETUP.md`.
