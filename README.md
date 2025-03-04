# Matplotlib_challenge
---

## Project Overview:

This project analyzes data from a pharmaceutical study conducted by Pymaceuticals, Inc., which specializes in anti-cancer treatments. The study evaluates the effectiveness of multiple drug regimens in treating squamous cell carcinoma (SCC) in mice.

---

## 📂 Files Included

### 1️⃣ Data Files (Located in `data/` Folder)

  - `Mouse_metadata.csv` → Contains individual-level data (e.g., Mouse ID, Drug Regime, and Sex).

  - `Study_results.csv` → Contains population-level data (e.g., Timepoint, Tumor Volume (mm<sup>3</sup>), and Metastic Sites).

### 2️⃣ Jupyter Notebook File

  - `Matplotlib_challenge.ipynb` → Contains code executed for data processing, analysis, and visualization.

---

## 📂 Repository Structure
```
Matplotlib_challenge
|── Pymaceuticals/
|  |── data/
|  |  |── Mouse_metadata.csv
|  |  |── Study_results.csv
|  |── Matplotlib_challenge.ipynb
|── .gitignore
|── README.md
```

---

## 🎯 Objective:

  -  Clean and preprocess the dataset.

  -  Perform exploratory data analysis and statistical summary.

  -  Visualize tumor volume distribution across different drug regimens.

  -  Identify outliers in the tumor volume dataset.

  -  Investigate the correlation between mouse weight and tumor volume.

  -  Perform a linear regression analysis to assess the relationship between mouse weight and tumor volume in the Capomulin regimen.

---

## 1️⃣ Dataset Information

Key Variables:

  - **Mouse ID**: Unique identifier for each mouse.

  - **Timepoint**: Days since the start of treatment.

  - **Tumor Volume (mm<sup>3</sup>)**: Tumor size at each timepoint.
  
  - **Drug Regimen**: Treatment administered to the mouse.

  - **Weight (g)**: Mouse weight in grams.

## 2️⃣ Data Cleaning

- Merged the `Mouse_metadata.csv` and `Study_results.csv` into a single DataFrame.

- Checked for duplicate timepoints and removed duplicated mouse data (Mouse ID: *g989*).

- Ensured consistency in the cleaned dataset before performing analysis.

## 3️⃣ Exploratory Data Analysis (EDA)

Summary Statistics:

- Calculated mean, median, variance, standard deviation, and SEM for tumor volume per drug regimen.

- Displayed results in a summary statistics table.

Data Visualizations:

- **Bar Charts** showed the number of observations for each drug regimen.

- **Pie Charts** displayed the gender distribution of mice in the study.

- **Box Plot of Tumor Volume** compared the distribution of final tumor volumes across the four most promising drug regimens:

    **Capomulin**

    **Ramicane**

    **Infubinol**

    **Ceftamin**

- Identified potential outliers in **Infubinol** and **Ceftamin**.

## 4️⃣ Capomulin Regimen Analysis

- **Line Plot:** Tracked tumor volume changes over time for a single mouse (Mouse ID: l509) treated with Capomulin.

- **Scatter Plot:** Examined the relationship between mouse weight and tumor volume in the Capomulin regimen.

## 5️⃣ Correlation & Regression Analysis

- Pearson Correlation Coefficient (r-value) → *0.84* (strong positive correlation between mouse weight and tumor volume).

- Linear Regression Model:
  - Equation:

        Tumor Volume = (slope × Mouse Weight) + intercept

  - Plotted a regression line on the scatter plot to visualize the trend.
  
  - P-value: Displayed to assess statistical significance.

---

## 🔍 Key Findings & Conclusion

✅ Capomulin & Ramicane were the most effective treatments, showing the smallest final tumor volumes.

✅ Infubinol & Ceftamin showed higher tumor volumes and had potential outliers, indicating lower effectiveness.

✅ Mouse weight was strongly correlated with tumor volume (r = 0.84).

✅ Linear regression confirmed a significant relationship between mouse weight and tumor volume.

---

## 📌 Final Recommendation:

Further research should focus on Capomulin and Ramicane as potential treatments for squamous cell carcinoma (SCC).

---

## 🧰 Required Dependencies

- Python 3+
- Jupyter Notebook
- Pandas (Data manipulations & analysis)
- Matplotlib (Data visualization)
- Scipy (Statistical analysis)

Ensure you have a Python version that is up to date and install the following in GitBash:

```
pip install pandas matplotlib scipy
```

---

## 🏎️ How to Run the Project

  1.) Clone this repository or download the files to your local machine.
  
  2.) Ensure your Python installed (Recommended: Python 3.8+)

  3.) Ensure the required libraries are installed in your operating environment.

  4.) Launch Jupyter Notebook and run the file cells sequentially (`Kernel` &#8594; `Run`)

## 🔗 References

- **Python Official Documentation**: https://docs.python.org/3/

- **Pandas Library**: https://pandas.pydata.org/

- **Matplotlib Library**: https://matplotlib.org/

- **SciPy Library**: https://scipy.org/

---
