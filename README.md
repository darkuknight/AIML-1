# Task 1: Data Cleaning & Preprocessing

## Objective
Learn how to clean and prepare raw data for machine learning using Python and common data science libraries.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset
- Titanic Dataset
- File used in the notebook: `../data/Titanic-Dataset.csv`

## Workflow

### 1. Import the dataset and explore basic information
The notebook begins by loading the dataset into a Pandas DataFrame and checking basic structure.

Typical checks include:
- `df.describe()`
- `df.head()` and `df.tail()`
- `df.info()`
- `df.isnull().sum()`

### 2. Handle missing values
Missing values are handled using simple imputation techniques.

Examples used in the notebook:
- Mean imputation for numeric columns such as `Age`
- Median imputation for numeric columns such as `Age`
- Filling missing categorical values such as `Embarked`

### 3. Convert categorical features into numerical values
Categorical columns are transformed into numbers so they can be used in ML models.

Examples:
- `Sex` mapped to binary values
- `Embarked` mapped to numeric labels

### 4. Normalize or standardize numerical features
Continuous features are standardized using Z-score normalization.

Columns normalized in the notebook:
- `Age`
- `Fare`

### 5. Visualize and remove outliers
Boxplots are used to detect outliers, followed by IQR-based filtering to remove them.

Columns analyzed for outliers:
- `Age`
- `Fare`

## Notebook Output
The notebook demonstrates the complete preprocessing pipeline step by step, making it easy to reuse the code for other datasets.

## How to Run
1. Open `data_preprocessing.ipynb` in VS Code or Jupyter.
2. Run the cells in order.
3. Inspect the plots and DataFrame outputs after each preprocessing step.

## Notes
- The dataset path is relative to the notebook location.
- Some preprocessing steps modify the DataFrame in place, so run the notebook from top to bottom for consistent results.