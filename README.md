# MDS Lab Practical Questions

This repository contains Jupyter Notebook solutions, viva notes, and small CSV
datasets for practical exercises in NumPy, Pandas, data preprocessing,
visualization, statistics, and machine learning.

## Contents

| Folder | Notebook questions | Main topics |
|---|---:|---|
| `Set-1` | Q1-Q4 | NumPy arrays, missing values, outliers, distributions, KNN |
| `Set-2` | Q5-Q8 | DataFrame operations, skewness, Min-Max scaling, correlation, SVM |
| `Set-3` | Q9-Q12 | NumPy indexing, categorical encoding, regression plots, decision trees |
| `Set-4` | Q13-Q16 | IQR outlier handling, correlation, feature importance, visualization, linear regression |
| `Set-5` | Q17-Q20 | NumPy operations, duplicate removal, histograms, logistic regression |
| `Set-6` | Q21-Q24 | Pandas transformations, imputation, standardization, trend plots, KNN comparison |
| `Set-7` | Q25-Q28 | Matrix operations, house-price visualization, category comparisons, linear regression |
| `Set-8` | Q29-Q32 | String operations, imputation, feature scaling, weather plots, SVM |
| `Extra_Substitute_Practical_Questions` | Q33-Q36 | House-price preprocessing, correlation, skewness transformation, plant-growth analysis |

Each numbered set contains:

- One `.ipynb` notebook with four practical questions
- CSV files used by the notebook
- A `Viva-SetN.md` file containing viva preparation material

The `Extra_Substitute_Practical_Questions` folder contains the substitute
notebook and its four supporting CSV datasets.

## Project Structure

```text
MDS_LAB/
├── Set-1/
│   ├── Set1.ipynb
│   ├── customers.csv
│   ├── marks.csv
│   └── Viva-Set1.md
├── Set-2/ ... Set-8/
├── Extra_Substitute_Practical_Questions/
│   ├── Extras.ipynb
│   ├── fitness.csv
│   ├── house_raw.csv
│   ├── income_skew.csv
│   └── plants.csv
├── .gitignore
└── README.md
```

## Requirements

- Python 3.9 or later
- Jupyter Notebook or JupyterLab
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

Install the required packages with:

```bash
python -m pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## Running the Notebooks

Clone the repository and start Jupyter from the project directory:

```bash
git clone <repository-url>
cd MDS_LAB
jupyter notebook
```

Open a notebook from its own set folder. The notebooks use relative paths such
as `pd.read_csv('customers.csv')`, so the notebook should be run with its
corresponding folder as the working directory. For example:

```bash
cd Set-1
jupyter notebook Set1.ipynb
```

The same approach applies to `Set-2` through `Set-8` and
`Extra_Substitute_Practical_Questions`.

## Topics Covered

- NumPy array creation, reshaping, slicing, arithmetic, and matrix operations
- Pandas DataFrames, ranking, sorting, grouping, mapping, and transformations
- Missing-value imputation and duplicate removal
- IQR-based outlier detection and replacement
- Label encoding, feature scaling, and skewness transformations
- Histograms, density plots, scatter plots, regression plots, bar charts,
  line charts, and heatmaps
- KNN, SVM, decision tree, logistic regression, and linear regression models
- Accuracy, confusion matrices, ROC curves, R², MSE, and residual analysis

## GitHub Notes

The notebooks and CSV files are small enough for normal GitHub rendering.
The Python virtual environment is intentionally excluded from version control
through `.gitignore`. Do not commit `.venv/`; dependencies should be installed
using the commands above.
