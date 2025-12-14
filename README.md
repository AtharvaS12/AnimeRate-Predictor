\# AnimeRate-Predictor



A machine learning pipeline to classify anime ratings into tiers (Score 6, 7, and 8) using metadata from MyAnimeList 2025.



\## 🚀 Workflow



\### 1. Data Preprocessing

\* \*\*Duration Parsing:\*\* Converts "min per ep" to numerical seconds.

\* \*\*Feature Expansion:\*\* Handles multi-label Genres, Themes, and Producers via One-Hot Encoding.

\* \*\*Cleaning:\*\* Sanitizes Rank and Popularity columns by removing special characters.



\### 2. Classification Modeling

\* \*\*Dimensionality Reduction:\*\* Uses PCA to manage 2,000+ generated features.

\* \*\*Outlier Handling:\*\* Implements Z-score imputation.

\* \*\*Algorithms:\*\* Compares Logistic Regression and Random Forest.

\* \*\*Best Performance:\*\* Random Forest achieved \*\*98% Accuracy\*\* using Decision Tree feature selection.



\## 📂 Files

\* `01\_Anime\_Data\_Preprocessing.ipynb`: From raw data to clean features.

\* `02\_Anime\_Rating\_Classification\_Model.ipynb`: Model training and benchmarking.



\## 🛠️ Requirements

`pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

