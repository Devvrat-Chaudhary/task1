##  Task 1: Data Cleaning & Preprocessing

###  Objective

To apply essential data preprocessing techniques to clean and prepare raw data (Titanic dataset) for machine learning tasks.

---

###  Dataset

**Name**: Titanic Dataset
**Source**: [Kaggle - Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
**File used**: `titanic.csv` (uploaded to `/content/` directory in Google Colab)

---

###  Tools & Libraries

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib & Seaborn** (for visualization)
* **Scikit-learn** (for preprocessing)

---

###  Steps Performed

1. **Importing Libraries & Dataset**

   * Loaded Titanic dataset into a Pandas DataFrame.

2. **Initial Data Exploration**

   * Inspected data types, missing values, and basic statistics.

3. **Handling Missing Values**

   * Imputed `Age` with median.
   * Filled `Embarked` with mode.
   * Dropped the `Cabin` column due to excessive missing data.
     
| Feature    | Method Used       | Comment                                                          |
| ---------- | ----------------- | ---------------------------------------------------------------- |
| `Age`      | Median Imputation | ✅ Good for skewed data and avoids outlier influence              |
| `Embarked` | Mode Imputation   | ✅ Reasonable for categorical features with few missing entries   |
| `Cabin`    | Dropped           | ✅ Acceptable if not more than 20-30% missing, but may lose useful information |


4. **Categorical Encoding**

   * Converted `Sex` using Label Encoding.
   * Applied One-Hot Encoding to `Embarked`.

5. **Feature Scaling**

   * Standardized `Age` and `Fare` using `StandardScaler`.

6. **Outlier Detection & Removal**

   * Visualized outliers using boxplots.
   * Removed outliers based on the IQR method.

7. **Final Dataset**

   * Verified clean structure and ensured all features are ready for modeling.

---

###  Key Concepts Learned

* Types of missing data and how to handle them
* Label Encoding vs One-Hot Encoding
* Normalization vs Standardization
* Outlier detection using boxplots and IQR
* Importance of preprocessing in ML pipelines

---

###  Output

A cleaned and preprocessed dataset ready for further model training and evaluation.

---

###  How to Run

1. Open the Colab notebook: `Task1_Data_Preprocessing.ipynb`
2. Upload `titanic.csv` to `/content/`
3. Run the notebook cells sequentially

---

###  Submission

Submission of the GitHub reporitory done on the given Link 
