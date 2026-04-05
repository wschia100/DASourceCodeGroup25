# CSC3105 Project

## Setup Instructions

Install all required dependencies before running any notebooks:

```bash
pip install -r requirements.txt
```

| Package | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical computing |
| `matplotlib` | Plotting and visualization |
| `seaborn` | Statistical data visualization |
| `scipy` | Signal processing (`find_peaks`) |
| `scikit-learn` | ML models, preprocessing, and evaluation |
| `xgboost` | Gradient boosting classifier |

---

## File Mapping to Assignment Components

Our files are organized to match the assignment questions and implementation flow:

- `a_Data_Preparation.ipynb` → **(a) Data Preparation/Preprocessing**
- `b_Data_Mining_Classification.ipynb` → **(b) Data Mining (Classification)**
- `b_Data_Mining_Regression.ipynb` → **(b) Data Mining (Regression)**

## Important Note

**There are no separate notebooks for parts (c) and (d).**

- **(c) Data Visualization is already integrated into** `a_Data_Preparation.ipynb`, `b_Data_Mining_Classification.ipynb`, and `b_Data_Mining_Regression.ipynb`.
- **(d) Result Analysis is already integrated into** `b_Data_Mining_Classification.ipynb` and `b_Data_Mining_Regression.ipynb`.

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

1. Integrated into Data Preparation and Data Mining notebooks (no standalone notebook).
2. Plots support preprocessing decisions and model evaluation.

### (d) Result Analysis

1. Integrated into Data Mining notebooks (no standalone notebook).
2. Includes model-level evaluation, interpretation, and justification.

## Repository Notes

- Input data is stored under `Input_Data/`.
- Trained model outputs are stored under `Output_Models/`.
- Large data/model artifacts are ignored via `.gitignore`, while folder structure is preserved with placeholder README files.
- For notebook output cleaning setup, see `TEAM_SETUP.md` *(for team use only).*

---

## Team Information

Group: **25**

| Team Member | UoG UID | SIT Student ID |
|---|---|---|
| Kenny Chin Aik Leck | 3070574L | 2403543 |
| Chia Wei Sheng | 3070620C | 2400953 |
| Low Lih Yih | 3070675L | 2402031 |
| Chen Junwei | 3070589C | 2400609 |
| Ong Tun Siang | 3070679O | 2402091 |