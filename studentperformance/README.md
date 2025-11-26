# Student Performance Dataset — Data Cleaning & Preprocessing

This project demonstrates data cleaning and preprocessing on the **Student Performance Dataset**.

---

## Dataset

- Source: Your CSV file (Student Performance Dataset)  
- 1000 rows, 8 columns:
  - `gender`
  - `race/ethnicity`
  - `parental_level_of_education`
  - `lunch`
  - `test_preparation_course`
  - `math_score`
  - `reading_score`
  - `writing_score`

---

## Steps Performed

### 1. Loaded and inspected the dataset
- Used `df.head()`, `df.info()`, and `df.describe()` to check:
  - Structure of the dataset
  - Data types
  - Basic statistics
  - Presence of missing values

### 2. Checked for missing values
- Checked for null values using `df.isnull().sum()`
- Checked for hidden missing values such as `" "` or `"na"`
- **Result:** No missing values found

### 3. Checked and removed duplicate rows
- Counted duplicates using `df.duplicated().sum()`
- Removed duplicates using `df.drop_duplicates()`
- **Result:** No duplicate entries

### 4. Standardized categorical columns
- Converted text to lowercase and stripped extra spaces
- Columns cleaned:
  - `gender`
  - `race/ethnicity`
  - `parental_level_of_education`
  - `lunch`
  - `test_preparation_course`
- **Result:** Consistent categorical values

### 5. Feature engineering
- Created `average_score` = mean of `math_score`, `reading_score`, `writing_score`
- Created `performance_level` based on average score:
  - 0–50 → Low
  - 50–75 → Medium
  - 75–100 → High

### 6. Outlier detection
- Detected outliers in `math_score`, `reading_score`, `writing_score` using IQR method
- Optionally, outliers can be removed or capped


---

## Final Dataset

- Contains cleaned and preprocessed columns ready for:
  - Analysis
  - Visualization
  - Machine learning
