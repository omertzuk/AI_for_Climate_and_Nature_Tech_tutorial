# AI for Climate & NatureTech — ML Tutorial

Hands-on machine learning tutorials for environmental conservation and monitoring.

**Instructor:** Dr. Omer Tzuk  
**Course:** AI for Climate & NatureTech (Microsoft Herzliya / University of Haifa)

## 🚀 Quick Start

Open the notebooks directly in Google Colab — no installation needed:

| Notebook | Colab Link |
|----------|------------|
| ML Demo (Regression, Clustering, Classification) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ukidH1mDhEOlm2BmR-y01qmGGyqwTrAF?usp=sharing) |
| HuggingFace Demo (NLP & Vision) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/113JJrQk0QbInUODn_u58ybmEeMGtxhO0?usp=sharing) |

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

| Notebook | Topics |
|----------|--------|
| `AI_for_Climate_NatureTech_ML_Demo.ipynb` | **Regression** (carbon stock prediction), **Clustering** (K-means + hierarchical), **Classification** (ecological status with Random Forest, SMOTE) |
| `AI_for_Climate_NatureTech_HuggingFace_Demo.ipynb` | **Sentiment Analysis** (IMDb reviews with DistilBERT), **Environmental Claims Detection** (ClimateBERT greenwashing detector), **Bird Species Classification** (EfficientNet-B2 image classifier) |

---

## 📓 Notebook 1 — ML Demo

### 🌲 Part 1 — Regression
Predict carbon stock in Israeli forest plots from environmental features using Random Forest. Includes a +2°C climate warming scenario.

### 🔍 Part 2 — Clustering
Discover ecological regions using K-means and hierarchical clustering — without ever showing the algorithm the region labels.

### 🌊 Part 3 — Classification
Classify river ecological status from catchment pressures, based on [Martyszunis et al. (2024)](https://doi.org/10.1038/s41598-024-74511-4). Demonstrates the SMOTE technique for imbalanced classes.

---

## 📓 Notebook 2 — HuggingFace Demo

### 🎬 Part A — Sentiment Analysis
Use a pre-trained DistilBERT model and fine-tune it on the IMDb movie reviews dataset. Demonstrates the HuggingFace `pipeline` API and the full train → evaluate → predict workflow.

### 🌿 Part B — Environmental Claims Detection (Greenwashing Detector)
Apply [ClimateBERT](https://huggingface.co/climatebert) — a language model pre-trained on 2M+ paragraphs of climate text — to detect real environmental claims in corporate reports vs. vague sustainability language. Based on [Stammbach et al. (2023)](https://arxiv.org/abs/2209.00507) and [Webersinke et al. (2022)](https://arxiv.org/abs/2110.12010).

### 🐦 Part C — Bird Species Classification
Classify bird species from photographs using an EfficientNet-B2 vision model fine-tuned on 525 species. Demonstrates that the same `pipeline` API works across text and images, connecting to biodiversity monitoring and citizen science applications.

---

## ⚙️ Setup
```bash
pip install -r requirements.txt
```

Or run everything in Google Colab (no local installation needed).

## 📚 References

- Martyszunis, A., Loga, M. & Przeździecki, K. (2024). Using machine learning for the assessment of ecological status of unmonitored waters in Poland. *Scientific Reports*, 14, 24509.
- Stammbach, D., Webersinke, N., Bingler, J.A., Kraus, M. & Leippold, M. (2023). Environmental Claim Detection. *arXiv:2209.00507*.
- Webersinke, N., Kraus, M., Bingler, J.A. & Leippold, M. (2022). ClimateBERT: A Pretrained Language Model for Climate-Related Text. *Proceedings of AAAI 2022 Fall Symposium*.
- Christin, S., Hervet, É. & Lecomte, N. (2019). Applications for deep learning in ecology. *Methods in Ecology and Evolution*, 10, 1632–1644.
- Pichler, M. & Hartig, F. (2023). Machine learning and deep learning: A review for ecologists. *Methods in Ecology and Evolution*, 14, 994–1016.