# 🎬 Netflix Data Preprocessing

This project focuses on data cleaning, feature transformation, and preparation of a dataset inspired by Netflix content. The goal is to create a clean, structured version of the dataset suitable for future machine learning tasks such as classification or recommendation systems.

---

## 📂 Project Structure
```
├── Data_Preprocessing_Netflix.ipynb # Jupyter notebook with all preprocessing steps
├── README.md # Project documentation
└── requirements.txt # Python dependencies
```
---

## 🧾 Dataset Overview

The dataset includes information about Netflix titles, such as:

- Title and description
- Genre and type (Movie or TV Show)
- IMDb score
- Runtime
- Cast (`stars`)
- Votes
- Binary indicator for Netflix original content

---

## 🔧 Preprocessing Summary

The following steps were completed:

- **Missing Values Handling**
  - Mode imputation for `genre`, `stars`
  - Mean imputation for `imdb`, `runtime`, `votes`

- **Encoding Categorical Features**
  - One-hot encoding for `type` and `genres`
  - Label encoding for `stars` and `original`

- **Outlier Detection and Handling**
  - Removed outliers from `runtime` and `imdb`
  - Replaced outliers in `votes` with the median value

- **Feature Scaling**
  - Tested StandardScaler, MinMaxScaler, and RobustScaler

---

## 📝 Next Steps

Future work will include:

- Model training for classification or recommendation
- Exploratory visualizations
- Model evaluation using metrics like accuracy, precision, recall, and F1-score

---

## ✅ Final Notes

This notebook sets a clean foundation for modeling and deeper analysis of streaming platform content. It demonstrates the importance of thoughtful data preparation before any machine learning workflow.

