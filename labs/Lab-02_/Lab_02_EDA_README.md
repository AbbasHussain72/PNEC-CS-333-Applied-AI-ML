
# 🔬 Lab 02: Exploratory Data Analysis (EDA) on Milling Dataset  
**Course:** CS-333 Applied AI & Machine Learning  

---

## 📌 1. Objective

The aim of this lab is to perform **Exploratory Data Analysis (EDA)** on a real-world milling dataset containing machining parameters, tool wear measurements, and multi-sensor signals.

Students will:

- Perform systematic data cleaning
- Handle missing values and duplicates
- Conduct statistical analysis
- Analyze distribution characteristics
- Detect and remove outliers
- Perform correlation analysis
- Visualize data using appropriate plots
- Understand the importance of EDA before applying Machine Learning models

---

## 📂 2. Dataset Description

The dataset (`mill.csv`) represents a real-world milling process monitoring scenario where tool wear and multiple sensor signals are recorded under different machining conditions. Each row corresponds to a single machining run.

The dataset includes:

### 🟢 Machining Parameters
- Machining time
- Depth of Cut (DOC)
- Feed rate
- Material type

### 🟠 Tool Condition
- **VB (Tool Flank Wear)** – Primary variable of interest

### 🔵 Sensor Signals
- Spindle motor currents (AC and DC)
- Vibration (Table and Spindle)
- Acoustic Emission (AE) (Table and Spindle)

This dataset simulates an industrial smart manufacturing environment where sensor data is used for tool condition monitoring and predictive maintenance.

---

## 🎯 3. Learning Outcomes

After completing this lab, students will be able to:

- Perform structured Exploratory Data Analysis
- Clean real-world noisy datasets
- Detect and handle missing values
- Identify duplicates
- Analyze center, spread, shape, and outliers
- Understand feature relationships using correlation
- Visualize engineering data effectively
- Explain why EDA is essential in AI/ML workflows

---

## 🧪 4. Lab Instructions

⚠️ **Important Guidelines**

- Each task must be performed under a separate section header.
- Every step should be executed in an individual notebook cell.
- All analytical explanations must be written in Markdown cells.

---

# 🔹 Task 1: Load the Dataset

### Steps:
- Import necessary libraries (pandas, numpy, matplotlib, seaborn)
- Load the dataset
- Display the first and last 5 rows
- Check data types
- Check dataset shape

---

# 🔹 Task 2: Data Cleaning

Ensure dataset quality before analysis.

### Steps:

1. **Check Missing Values**
   - Identify missing values
   - Fill missing values using an appropriate method discussed in class

2. **Check Duplicate Records**
   - Identify duplicate rows
   - Remove duplicate records

3. **Ensure Correct Data Types**
   - Convert columns to appropriate numerical types where necessary

---

# 🔹 Task 3: Statistical Analysis

Students must compute the following for all numerical columns:

## 1️⃣ Center (Typical Value)
- Mean  
- Median  
- Mode  

Answer in Markdown:
- Is tool wear normally distributed?
- Is the mean close to the median?

## 2️⃣ Spread (Variation)
- Standard Deviation  
- Variance  
- Range (Max − Min)  
- Interquartile Range (IQR = Q3 − Q1)

Answer in Markdown:
- Which sensor shows the highest variability?
- Does vibration vary more than current?

## 3️⃣ Shape (Distribution Pattern)
- Histogram  
- KDE Plot  
- Skewness  
- Kurtosis  

Answer in Markdown:
- Is the distribution symmetric?
- Is it right-skewed or left-skewed?
- Is it multi-modal?

## 4️⃣ Outlier Detection
Use:
- Boxplots  
- IQR Method  
- Modified Z-score  

After detecting outliers:
- Remove them using a justified method.
- In a separate Markdown cell, explain:
  - Which method was selected
  - Why it was selected
  - Which parameters contain significant outliers
  - How removal affected dataset statistics

---

# 🔹 Task 4: Correlation Analysis

- Compute correlation matrix (for all numerical features)
- Plot correlation heatmap

Answer in Markdown:
- Does tool wear strongly correlate with vibration?
- Which sensor appears most predictive of tool wear?
- Are any features redundant?

---

# 🔹 Task 5: Data Visualization

Create:
- Histogram (Tool Wear)
- Boxplot (Sensor Comparison)
- Scatter Plot (Tool Wear vs Vibration)
- Correlation Heatmap
- Pairplot (Optional – Advanced)

Visualizations must support engineering conclusions.

---

# 🧠 5. Engineering Thinking Questions

Answer in Markdown:

1. Which parameter affects tool wear the most?
2. Which sensor signal is most stable?
3. Are there abnormal machining cycles?
4. Can tool wear be predicted from sensor data?
5. If building a Machine Learning model, which features would you select?

---

# 📦 Submission Requirements

Students must submit:

- Completed Jupyter/Colab notebook
- All required plots
- Clear Markdown explanations
- Cleaned dataset (if modified)

---

# 🚀 Why EDA is Important

Exploratory Data Analysis is the foundation of any AI/ML pipeline. Without proper EDA:

- Models may learn incorrect patterns
- Noise and outliers may distort results
- Wrong assumptions may lead to poor predictions

EDA ensures clean and reliable data, better feature selection, improved model performance, and engineering insight before automation.

---

# 🏁 Expected Outcome

By the end of this lab, students should:

✔ Understand industrial sensor data  
✔ Perform structured EDA  
✔ Detect anomalies  
✔ Interpret statistical measures  
✔ Prepare data for Machine Learning  
