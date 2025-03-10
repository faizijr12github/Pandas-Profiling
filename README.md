# 📊 Pandas Profiling (ydata-profiling)

**Automate Exploratory Data Analysis (EDA) with Pandas Profiling!**

## 🚀 Introduction
[Pandas Profiling](https://github.com/ydataai/ydata-profiling) (now **ydata-profiling**) is a powerful Python library for generating **detailed and interactive** reports on datasets with minimal code. It helps in understanding data distribution, missing values, correlations, and more.

## 📌 Installation
To install Pandas Profiling, run:
```bash
pip install ydata-profiling
```

## 🛠️ Usage

### 1️⃣ **Basic Usage**
```python
import pandas as pd
from ydata_profiling import ProfileReport

# Load dataset
df = pd.read_csv("your_dataset.csv")  # Replace with your actual file

# Generate Profile Report
profile = ProfileReport(df, explorative=True)

# Save report as an HTML file
profile.to_file("EDA_Report.html")

# Display in Jupyter Notebook
profile.to_notebook_iframe()
```

### 2️⃣ **Customizing the Report**
You can configure the report with custom settings:
```python
profile = ProfileReport(df, title="My Data Report",
                        explorative=True, minimal=True)
```
- `explorative=True`: Enables an interactive report.
- `minimal=True`: Generates a **lightweight** report (faster for large datasets).

## 📌 Features
✅ **Overview**: Dataset info, variable types, and duplicate rows.  
✅ **Missing Values**: Heatmaps and percentage of missing data.  
✅ **Data Distribution**: Histograms, boxplots, and statistics.  
✅ **Correlations**: Pearson, Spearman, and Kendall correlation heatmaps.  
✅ **Warnings**: Identifies potential data issues.  
✅ **Exportable**: Save reports as **HTML**, **JSON**, or **Markdown**.


