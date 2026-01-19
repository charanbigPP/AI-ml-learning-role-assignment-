# Exploratory Data Analysis & Machine Learning on Iris Dataset

This project applies **Exploratory Data Analysis (EDA)** and **Logistic Regression** to the classic Iris dataset to classify flower species. It is designed as a clean, beginner-friendly machine learning project showcasing the complete workflow from data exploration to model evaluation, optimized for **Google Colab**.

## 📌 Objective

* Understand the Iris dataset through comprehensive EDA.
* Build a classification model to predict the species (Setosa, Versicolor, Virginica).
* Demonstrate best practices in data preprocessing, visualization, and model evaluation.

## 📊 Dataset

* **Dataset:** Sklearn Built-in Iris Dataset
* **Task:** Multi-class classification (3 species)
* **Target Variable:** `species` (0: Setosa, 1: Versicolor, 2: Virginica)
* **Key Features:**
* Sepal length (cm)
* Sepal width (cm)
* Petal length (cm)
* Petal width (cm)



## 🛠️ Tools & Technologies

* **Language:** Python 3.x
* **Libraries:** * `pandas` & `numpy` - Data manipulation
* `matplotlib` & `seaborn` - Data visualization
* `scikit-learn` - Machine learning and evaluation


* **Environment:** Google Colab / Jupyter Notebook

## 🚀 How to Run the Project

Since this project is optimized for Google Colab, no local installation is required.

1. **Open Google Colab:** Go to [colab.research.google.com](https://colab.research.google.com/).
2. **Upload/Paste the Code:** Create a new notebook and paste the provided Python code.
3. **Run All Cells:** Execute the cells in order to reproduce the analysis and results.

---

## 📈 Modeling Details

### Data Preprocessing

* **Loading:** Data is loaded directly from `sklearn.datasets`.
* **Cleaning:** Verified missing values using `df.isnull().sum()` (0 missing values found).
* **Feature Selection:** All four physical measurements were used as predictors (`X`).

### Train-Test Split

* **Training set:** 80%
* **Test set:** 20%
* **Random State:** 42 (for reproducibility)

### Model

* **Algorithm:** Logistic Regression
* **Configuration:** `LogisticRegression(max_iter=200, random_state=42)`

---

## 📊 Results & Interpretation

### Model Performance

* **Model Accuracy:** 1.0000 (100% on the test set)

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
| --- | --- | --- | --- | --- |
| Setosa (0) | 1.00 | 1.00 | 1.00 | 10 |
| Versicolor (1) | 1.00 | 1.00 | 1.00 | 9 |
| Virginica (2) | 1.00 | 1.00 | 1.00 | 11 |

**Key Insights:**

* The model achieves perfect classification on the test set.
* **Setosa** is the most easily distinguishable species due to its unique petal dimensions.

---

## 🔍 Exploratory Data Analysis Highlights

### Visualizations Created

1. **Pair Plot:** Visualized the pairwise relationships between all features colored by species.
2. **Box Plots:** Analyzed the distribution and outliers of each feature per species.
3. **Correlation Heatmap:** Identified strong relationships between Petal Length and Petal Width.

### Key EDA Findings

* **Petal Measurements:** Petal length and width show the strongest separation between species.
* **High Correlation:** Petal length and petal width have a very high positive correlation (0.96).
* **Distribution:** Species 0 (Setosa) has significantly smaller petals compared to the other two.

---

## ⚠️ Limitations & Future Improvements

* **Small Dataset:** The Iris dataset is very small (150 rows), which can lead to "perfect" scores that may not occur in larger, messier real-world data.
* **Future Improvement:** Implement **K-Fold Cross-Validation** to ensure the model's robustness.
* **Future Improvement:** Compare performance with other algorithms like **Decision Trees** or **K-Nearest Neighbors (KNN)**.

---

## 🎓 Author

Charan E

Location: bileshivale bangalore,karnataka

Focus: Machine Learning, Python Development

