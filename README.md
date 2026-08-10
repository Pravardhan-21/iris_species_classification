# Iris Species Classification using Machine Learning

A beginner-friendly machine learning project that explores the classic **Iris flower dataset**,
performs exploratory data analysis (EDA), and builds a classification model to predict the
species of an iris flower from its sepal and petal measurements.

## 📌 Project Overview

- ✅ Explore the Iris Dataset
- ✅ Perform Exploratory Data Analysis (EDA)
- ✅ Build a Machine Learning Classification Model

The Iris dataset contains 150 samples of iris flowers, evenly split across three species:

- *Iris-setosa*
- *Iris-versicolor*
- *Iris-virginica*

Each sample has four numerical features: `SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`,
and `PetalWidthCm`.

```

## 📝 Tasks Completed

### 1️⃣ Kaggle Setup
The dataset used is the well-known [Iris Species dataset on Kaggle](https://www.kaggle.com/datasets/uciml/iris).

### 2️⃣ Exploratory Data Analysis (EDA)
- Loaded the dataset with pandas
- Checked dataset info (`df.info()`) — data types and non-null counts
- Checked for missing values — the dataset has **zero** missing values
- Displayed summary statistics with `df.describe()`
- Created **6 visualizations**:
  1. Count plot of species distribution
  2. Pairplot of all features colored by species
  3. Correlation heatmap of numerical features
  4. Boxplots of each feature grouped by species
  5. Histograms of feature distributions
  6. Violin plot of petal length by species

### 3️⃣ Machine Learning Model
Built a **Random Forest Classifier** to predict species from the four numerical features.
(Random Forest was chosen over a single Decision Tree for improved robustness and accuracy,
while remaining fast and easy to interpret via feature importances.)

### 4️⃣ Model Evaluation
The model is evaluated on a held-out 20% test split using:
- **Accuracy Score**
- **Confusion Matrix** (visualized as a heatmap)
- **Classification Report** (precision, recall, F1-score per class)

On the test split, the model achieves **~90–100% accuracy** (exact value may vary slightly
depending on the random train/test split and can be reproduced by re-running the notebook).

## 🚀 How to Run

1. **Clone/download this project** and make sure `data/Iris.csv` is present.

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter:**
   ```bash
   jupyter notebook Iris_Classification.ipynb
   ```

4. **Run all cells** (Kernel → Restart & Run All) to reproduce the EDA, model training, and
   evaluation results.

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| pandas | Data loading and manipulation |
| numpy | Numerical operations |
| matplotlib / seaborn | Data visualization |
| scikit-learn | Model building and evaluation |
| Jupyter Notebook | Interactive development environment |
