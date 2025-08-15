## Data Cleaning and Manipulation

In this project, the marketing dataset was preprocessed to ensure clean and consistent data for analysis and visualize . 

###  General Dataset Settings
- Display settings were adjusted to show all columns for inspection using:
  ```python
  pd.set_option('display.max_columns', None)

###  Cleaning Whitespace, Dots, and Special Characters

Values in cells were cleaned to remove unnecessary whitespace, dots (.), and other special characters to ensure consistency.

This helped prevent errors during analysis and numeric computations.

###  Dropping Unnecessary Columns Safely
- Columns that were irrelevant for analysis or contained mostly missing values (e.g., `job`, `default`, `education`) were removed.  
- The `errors='ignore'` parameter was used to avoid errors if any column was already missing.

###  Recategorizing Categorical Columns

Columns like job and education were regrouped into more meaningful categories for easier visualization and modeling.

###  Renaming Columns

Certain column names were updated for clarity and consistency.

For example, job_grouped was renamed to job and education_grouped to education.

###  Handling Missing or “unknown” Values

Categorical columns contained unknown entries.

Depending on the analysis, these values were either removed if minimal or converted into a separate category (no_info) to preserve information.

Example: In the loan column, the 2.4% of unknown values were retained as a separate category.

###  Cleaning Whitespace, Dots, and Special Characters

Values in cells were cleaned to remove unnecessary whitespace, dots (.), and other special characters to ensure consistency.

This helped prevent errors during analysis and numeric computations.
