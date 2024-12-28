# 🚗 Used Cars Dataset Analysis  

## 📌 Project Overview  
This project focuses on analyzing a large dataset of used cars from Craigslist to extract insights, clean data, and prepare it for exploratory and predictive analysis. The dataset was processed to remove inconsistencies, handle missing data, and standardize information, enabling meaningful exploration and analysis.  

---

## 🛠️ Data Cleaning Process  
1. **Column Selection:**  
   - Irrelevant columns such as `url`, `region_url`, `VIN`, `description`, and `image_url` were removed.  

2. **Handling Missing Values:**  
   - Columns with more than 50% missing values were dropped.  
   - For categorical columns, missing values were replaced with `'Unknown'`.  
   - For numerical columns, missing values were replaced with the median.  

3. **Outlier Removal:**  
   - Price values outside the range of \$500 to the 99th percentile were excluded.  
   - Odometer readings above the 99th percentile were filtered out.  

4. **Data Standardization:**  
   - Categorical fields like `condition`, `fuel`, `transmission`, `drive`, and `paint_color` were standardized to lowercase.  

5. **Feature Engineering:**  
   - New columns such as `vehicle_age` and `posting_year` were derived to enhance analysis capabilities.  

6. **Deduplication:**  
   - Duplicate records were removed to ensure data integrity.  

---

## 🔍 Exploratory Data Analysis (EDA)  
- Summary statistics were calculated to understand the distribution of features.  
- Key relationships between attributes like `price`, `year`, `odometer`, and `manufacturer` were explored.  
- Patterns in categorical features such as `fuel` type and `transmission` were visualized.  

---

## 📂 Dataset Information  
- **Source:** Craigslist Cars and Trucks Dataset  
- **Number of Records:** 426,880 (before cleaning)  
- **Key Features:**  
  - `price`: Listing price of the vehicle  
  - `year`: Manufacturing year  
  - `condition`: Vehicle condition  
  - `fuel`: Fuel type  
  - `odometer`: Mileage of the vehicle  
  - `type`: Vehicle type (e.g., SUV, sedan)  
  - `paint_color`: Exterior color  

---

## 🔧 Tools & Libraries  
- **Languages:** Python  
- **Libraries Used:**  
  - `pandas` for data manipulation  
  - `numpy` for numerical operations  
  - `matplotlib` and `seaborn` for visualizations  

---

