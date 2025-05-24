# Nutrition-Predictor

A machine learning project using a **Random Forest Classifier** to analyze and classify nutritional values from the **Open Food Facts** dataset.

## 🎯 Objective

The primary aim is to uncover nutritional patterns, categorize food items, and provide dietary recommendations based on user input. The project leverages a dataset of over **104,000 entries** and **98 features**.

---

## 🛠️ Key Steps

### 1. Installation and Configuration
- Install the necessary Python libraries for data handling and AWS S3 access.
- Configure the AWS S3 client to read Excel files directly into Pandas DataFrames for efficient data processing.

### 2. Data Processing and Cleaning
- Define functions to:
  - Ensure required columns are present.
  - Handle missing values.
- Clean and standardize the data by:
  - Removing duplicates.
  - Selecting relevant columns (`nutrients_to_check`).
- Concatenate processed DataFrames into a master DataFrame for consistency.

### 3. Clustering Analysis
- Remove outliers using the **Z-Score** method.
- Apply **Principal Component Analysis (PCA)** to reduce dimensionality.
- Use the **elbow method** to determine the optimal number of clusters.
- Implement **K-Means clustering** to categorize nutritional data.
- Visualize clusters using **scatter plots**.

### 4. Diet Classification
- Define popular fad diets (e.g., Keto, low-carb) using established nutritional criteria.
- Normalize data using **StandardScaler**.
- Perform clustering with **12 clusters** using K-Means.
- Split data into **training and testing sets** using `train_test_split`.
- Train a **Random Forest Classifier** to classify nutritional profiles.
- Allow user input to:
  - Match nutritional habits with diet categories.
  - Generate personalized dietary recommendations.
- Visualize diet alignment through **bar charts**.

---

## ✅ Expected Outcomes

- **Enhanced Understanding**: Discover nutritional patterns and trends via clustering and classification.
- **Personalized Recommendations**: Tailored diet suggestions based on user input.
- **Data Visualization**: Clear visuals for interpreting complex data relationships.

---

## 📚 References and Data Sources

- [Open Food Facts Database](https://world.openfoodfacts.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib API](https://matplotlib.org/stable/contents.html)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [NumPy Documentation](https://numpy.org/)
- [SciPy z-score Reference](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.zscore.html)
- [Scikit-learn Clustering](https://scikit-learn.org/stable/modules/clustering.html)
- [Scikit-learn Supervised Learning](https://scikit-learn.org/stable/supervised_learning.html)
- [Scikit-learn KMeans](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
- [Scikit-learn RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [PrettyTable Google Code](https://code.google.com/archive/p/prettytable/)
- [Nutrition.gov](https://www.nutrition.gov/)
- [Health.gov Dietary Guidelines](https://health.gov/dietary-guidelines/)
- [AZoM Article on Nutrition](https://www.azom.com/)
- [LibreTexts on Modified Diets](https://med.libretexts.org/)
- [Wikipedia List of Diets](https://en.wikipedia.org/wiki/List_of_diets)
- [Healthy Eating Index (HEI) Scoring](https://www.fns.usda.gov/)
- [NIH: Vitamins and Minerals for Older Adults](https://www.nia.nih.gov/)
- [Harvard Health: Listing of Vitamins](https://www.health.harvard.edu/)

---

