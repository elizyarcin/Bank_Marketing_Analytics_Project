# 📊 Bank Marketing Analytics Project

This project analyzes a bank marketing dataset to discover insights about customer behavior and campaign performance.  
It includes **data cleaning**, **feature engineering**, and **visualization** steps to prepare for deeper analysis and potential predictive modeling.

---

## 🧹 Data Cleaning and Manipulation

The dataset was preprocessed to ensure clean and consistent data for analysis and visualization.

### 🔧 General Dataset Settings
- Display settings were adjusted to show all columns for inspection:
  ```python
  pd.set_option('display.max_columns', None)

### ✨ Cleaning Whitespace, Dots, and Special Characters

Removed unnecessary whitespace, dots (.), and other special characters from cell values.

Ensured text fields are consistent and numeric columns are error-free.

### 🗑 Dropping Unnecessary Columns Safely

Removed irrelevant or mostly missing columns (job, default, education).

Used errors='ignore' to avoid runtime errors if the columns were already absent.

### 🗂 Recategorizing Categorical Columns

Grouped job and education categories into broader, more meaningful groups for simpler visualization and analysis.

### 🏷 Renaming Columns

Renamed columns for clarity and consistency:

job_grouped ➡️ job

education_grouped ➡️ education

### ❓ Handling Missing or “unknown” Values

For categorical columns with minimal unknown values, entries were either:

### Removed completely, or Converted into a separate no_info category to preserve data volume.

Example: In the loan column, 2.4% unknown values were labeled no_info.
