# Statistical Comparison of Forecasting Models for Land Surface Temperature (LST) in Nigeria

The study assesses their predictive performance in forecasting **Land Surface Temperature (LST) across Nigerian states** using RMSE values.This repository contains data, scripts, and plots for the **statistical evaluation of three forecasting models**:

- **Curve Fit Forecast**
- **Exponential Smoothing Forecast**
- **Forest-Based Forecast**

The study assesses their predictive performance in forecasting **Land Surface Temperature (LST) across Nigerian states** using RMSE values.

---

## 📂 Repository Structure

- [**data/**](/data/) → # Input datasets (RMSE values
- [**plot/**](datafile/) → # Generated figures (model performance heatmap, CD diagram, etc.) 
- [**script/**](script/) → # Analysis scripts (Friedman test, Nemenyi post-hoc test, etc.)  
- [**README.md**](README.md) → # Project documentation

---

# Statistical Analysis

To evaluate whether the models differed significantly in predictive performance:

### Friedman Test
- **Chi-Square statistic**: 47.19  
- **p-value**: < 0.0001  

Strong rejection of the null hypothesis → Not all models performed equally.

---

### Nemenyi Post-Hoc Test

| Model Comparison | p-value   | Significance |
|------------------|-----------|--------------|
| Curve Fit vs. Exponential Smoothing | 0.00000 | Significant |
| Curve Fit vs. Forest-Based Forecast | 0.00000 | Significant |
| Exponential Smoothing vs. Forest-Based Forecast | 0.18901 | Not significant |

---

## Key Findings

- **Curve Fit** performed **significantly worse** than both Exponential Smoothing and Forest-Based Forecast.  
- **Exponential Smoothing** and **Forest-Based Forecast** showed **comparable performance** (no significant difference).  
- Ensemble/advanced approaches (**Exponential Smoothing & Forest-Based**) are **more reliable for LST prediction** than Curve Fit.  

---

## Critical Distance (CD) Diagram

To visualize the average ranks and statistical significance, a **Critical Distance diagram** was generated using the Nemenyi test.  
- The diagram shows that **Exponential Smoothing** and **Forest-Based Forecast** are statistically similar, while **Curve Fit** stands apart with worse performance.

---

## Output Visualizations
- Heatmap of Nemenyi Post-Hoc Test → [View Here](plots/heatmap.png)
- Critical Difference Diagram → [View Here](plots/Critical_Difference_Diagram.png)

---

## Citation

If you use this repository, please cite it as:

Waheeb, T.B.. (2025). Statistical Comparison of Forecasting Models for Land Surface Temperature (LST) in Nigeria. GitHub repository. 

---

## How to Reproduce

Clone the repository:
   ```bash
   git clone https://github.com/bherney/Statistical-Comparison-of-Forecasting-Models-for-Land-Surface-Temperature.git
   cd Statistical-Comparison-of-Forecasting-Models-for-Land-Surface-Temperature

