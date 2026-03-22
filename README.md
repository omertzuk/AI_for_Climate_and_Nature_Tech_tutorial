# AI for Climate & NatureTech — ML Tutorial

Hands-on machine learning tutorials for environmental conservation and monitoring.

**Instructor:** Dr. Omer Tzuk  
**Course:** AI for Climate & NatureTech (Microsoft Herzliya / University of Haifa)

## 🚀 Quick Start

Open the notebook directly in Google Colab — no installation needed:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ukidH1mDhEOlm2BmR-y01qmGGyqwTrAF?usp=sharing)

## 📁 Contents

### Datasets

Each dataset is available in both CSV and Excel formats.

| File | Description |
|------|-------------|
| `datasets/israeli_forest_monitoring_dataset.csv` | 200 synthetic forest plots across 5 Israeli regions (Carmel, Upper/Lower Galilee, Judean Hills, Yatir Edge) with climate, vegetation, and fire data |
| `datasets/israeli_forest_monitoring_dataset.xlsx` | Same dataset in Excel format |
| `datasets/water_body_ecological_status_dataset.csv` | 800 synthetic river water bodies with catchment pressure data, modeled on the EU Water Framework Directive classification system |
| `datasets/water_body_ecological_status_dataset.xlsx` | Same dataset in Excel format |

### Notebooks

| Notebook | ML Tasks |
|----------|----------|
| `AI_for_Climate_NatureTech_ML_Demo.ipynb` | **Regression** (carbon stock prediction), **Clustering** (K-means + hierarchical), **Classification** (ecological status with Random Forest, SMOTE) |

## 🌲 Part 1 — Regression
Predict carbon stock in Israeli forest plots from environmental features using Random Forest. Includes a +2°C climate warming scenario.

## 🔍 Part 2 — Clustering
Discover ecological regions using K-means and hierarchical clustering — without ever showing the algorithm the region labels.

## 🌊 Part 3 — Classification
Classify river ecological status from catchment pressures, based on [Martyszunis et al. (2024)](https://doi.org/10.1038/s41598-024-74511-4). Demonstrates the SMOTE technique for imbalanced classes.

## ⚙️ Setup
```bash
pip install -r requirements.txt
```

Or run everything in Google Colab (no local installation needed).

## 📚 References

- Martyszunis, A., Loga, M. & Przeździecki, K. (2024). Using machine learning for the assessment of ecological status of unmonitored waters in Poland. *Scientific Reports*, 14, 24509.
- Christin, S., Hervet, É. & Lecomte, N. (2019). Applications for deep learning in ecology. *Methods in Ecology and Evolution*, 10, 1632–1644.
- Pichler, M. & Hartig, F. (2023). Machine learning and deep learning: A review for ecologists. *Methods in Ecology and Evolution*, 14, 994–1016.
