# 🧹 Data Cleaning Project

This project demonstrates a step-by-step **data cleaning workflow** using Python and Pandas on the `sales_data_sample.csv` dataset.  
The goal was to preprocess the dataset, handle missing values, correct data types, and remove duplicates to prepare it for further analysis.

---

## 📂 Tasks Performed

### 1. Importing Libraries
- Used **NumPy** and **Pandas** for data handling.

### 2. Loading Data
- Loaded the dataset `sales_data_sample.csv` with `latin1` encoding to handle special characters.

### 3. Initial Exploration
- Displayed the **first** and **last** few rows (`head()`, `tail()`).
- Checked **shape** (rows × columns).
- Verified **data types** (`dtypes`, `info()`).

### 4. Handling Missing Values
- Identified missing values using `isnull().sum()`.
- Dropped unnecessary columns:  
  - `ADDRESSLINE2`  
  - `STATE`  
  - `TERRITORY`  
- Dropped rows with missing **POSTALCODE** values.

### 5. Duplicate Handling
- Checked for duplicates using `duplicated().sum()`.

### 6. Data Type Conversions
- Converted `ORDERDATE` to **datetime** format.
- Cleaned and converted `PHONE` column:
  - Converted to **string**.  
  - Removed dots (`.`) and unwanted characters.  
  - Converted to **numeric** with invalid entries coerced to `NaN`.  
  - Dropped rows where `PHONE` remained `NaN`.

### 7. Final Dataset
- Printed the final shape of the cleaned dataset.

---

## 📊 Summary
- Dataset loaded, cleaned, and prepared for analysis.  
- Missing values and duplicates handled.  
- Columns standardized with correct datatypes.  

---

## 🚀 Next Steps couble be
- Perform **Exploratory Data Analysis (EDA)**.  
- Create **visualizations** (heatmaps, distributions, etc.).  
- Build predictive models using the cleaned dataset.

---

## 🛠️ Technologies Used
- Python 🐍  
- Pandas  
- NumPy  

---

## 📌 How to Run
1. Clone this repository  
   ```bash
   git clone https://github.com/yourusername/data-cleaning.git
   ```
2. Install dependencies  
   ```bash
   pip install pandas numpy
   ```
3. Run the script  
   ```bash
   python Data_Cleaning_Code.py
   ```

---

✨ **Author:** Pratik Kumar  
📅 **Project Type:** Data Cleaning & Preprocessing  
