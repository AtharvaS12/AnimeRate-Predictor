readme_content = """# ⛩️ AnimeRate-Predictor

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Accuracy](https://img.shields.io/badge/Accuracy-98%25-green.svg)](#)

A high-performance machine learning pipeline designed to classify anime ratings into tiers (**Scores 6, 7, and 8**) using metadata from MyAnimeList 2025. This project bridges the gap between raw entertainment metadata and predictive analytics.

---

## 🚀 Workflow Architecture

### 1. Data Preprocessing & ETL
* **Duration Parsing:** Advanced string parsing to convert "min per ep" formats into numerical total seconds for standardized comparison.
* **Feature Expansion:** Optimized handling of multi-label attributes (Genres, Themes, and Producers) using **One-Hot Encoding**, expanding the feature space to capture niche metadata.
* **Sanitization:** Cleaning of `Rank` and `Popularity` columns to remove non-numeric artifacts and handle missing values.

### 2. Classification Strategy
* **Dimensionality Reduction:** Utilized **Principal Component Analysis (PCA)** to condense 2,000+ sparse features, preventing the "curse of dimensionality."
* **Outlier Management:** Implemented **Z-score imputation** to ensure statistical robustness against extreme metadata values.
* **Modeling & Benchmarking:** Rigorous comparison between **Logistic Regression** (baseline) and **Random Forest** (ensemble).
* **Performance:** The **Random Forest** model achieved a peak **98% Accuracy**, significantly benefiting from Decision Tree-based feature importance selection.

---

## 📂 Project Structure

| File | Description |
| :--- | :--- |
| `01_Anime_Data_Preprocessing.ipynb` | End-to-end data cleaning, feature engineering, and ETL processes. |
| `02_Anime_Rating_Classification_Model.ipynb` | Training, PCA implementation, and hyperparameter tuning. |

---

## 🛠️ Technical Stack

* **Core:** `Python`, `NumPy`, `Pandas`
* **ML:** `Scikit-Learn` (PCA, Random Forest, Logistic Regression)
* **Visualization:** `Matplotlib`, `Seaborn`

---

## 📈 Results & Insights

* **Accuracy:** 98% (Random Forest)
* **Key Features:** `Popularity`, `Rank`, and specific `Studio/Producer` metadata were identified as the strongest predictors for high-tier ratings.
* **Inference:** The model excels at distinguishing between "cult classics" (Tier 7) and "seasonal hits" (Tier 8).

---

## ⚙️ Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/AnimeRate-Predictor.git](https://github.com/yourusername/AnimeRate-Predictor.git)