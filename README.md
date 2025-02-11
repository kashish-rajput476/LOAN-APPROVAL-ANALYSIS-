
 **Loan Approval Data Analysis – Exploratory Data Analysis (EDA)**  

### **Project Overview:**  
This project performs an exploratory data analysis (EDA) on a loan approval dataset. The objective is to clean, process, and visualize the data to uncover insights into factors affecting loan approvals. The analysis includes handling missing values, detecting outliers, feature engineering, and visualizing relationships between variables.  

---

## **Key Features of the Analysis:**  

### **1. Data Preprocessing:**  
- Loaded the dataset and checked for missing values.  
- Handled missing categorical values using the **mode** (most frequent value).  
- Filled missing numerical values using the **median** to reduce the impact of outliers.  

### **2. Outlier Detection & Removal:**  
- Used **Z-score normalization** to identify and remove extreme values in income and loan amounts.  
- This ensures that extreme values do not affect statistical trends in the dataset.  

### **3. Feature Engineering:**  
- Created a new column **"Total_Income"** by adding **ApplicantIncome** and **CoapplicantIncome** to get a better representation of financial strength.  
- Computed the **Loan_Income_Ratio** to evaluate how large the loan amount is compared to the total income.  

---

## **4. Data Visualization & Interpretation:**  

### **Univariate Analysis:** (Analyzing single variables)  
✔ **Income Distributions:**  
- Histograms for **ApplicantIncome**, **CoapplicantIncome**, and **LoanAmount** show their spread and skewness.  
- A **boxplot** for LoanAmount identifies outliers affecting loan distribution.  

✔ **Categorical Variables:**  
- Count plots for **Education** and **Property_Area** reveal the distribution of applicants based on their education and residential area.  
- **Gender distribution pie chart** shows the percentage of male vs. female applicants.  

### **Bivariate Analysis:** (Analyzing relationships between two variables)  
✔ **Loan Amount vs. Credit History:**  
- A boxplot shows that applicants with a **good credit history (1)** generally receive **higher loan amounts** than those with a bad credit history (0).  

✔ **Loan Approval by Education Level and Credit History:**  
- A **stacked bar chart** visualizes how education and credit history together impact loan approvals.  

### **Multivariate Analysis:**  
✔ **Pairplot:**  
- Shows relationships between numerical variables, color-coded by **Education**, to identify trends.  

✔ **Correlation Heatmap:**  
- Displays correlations between numeric features.  
- **LoanAmount** has a strong correlation with **Total_Income**, confirming the importance of financial stability in loan approval.  

---

## **Libraries Used:**  
✅ **Pandas, NumPy** – Data processing & manipulation  
✅ **Matplotlib, Seaborn** – Data visualization  
✅ **SciPy** – Statistical calculations  


## **How to Use This Project:**  
1️⃣ Run the script to load the dataset and process the data.  
2️⃣ View the **cleaned data** after handling missing values and outliers.  
3️⃣ Analyze insights from visualizations to understand **factors affecting loan approvals**.  

This project provides a structured approach to analyzing loan applications and can be used for financial decision-making or predictive modeling.  
