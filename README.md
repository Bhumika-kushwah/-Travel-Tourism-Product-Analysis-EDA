
# ✈️ Travel & Tourism Product Analysis – EDA

## 🔍 Project Overview
This project focuses on performing Exploratory Data Analysis (EDA) on a Travel & Tourism dataset to uncover customer behavior patterns, product conversion trends, and travel preferences.

The objective is to identify which customers are more likely to purchase travel packages and understand the business factors influencing travel conversions.

---

## 📁 Dataset Information
- Source: Kaggle – Travel.csv  
- Total Raw Records: 4,888 customers  
- Records After Cleaning: 4,128 customers  
- Features: 20 Columns  

### Key Features Used
- Age  
- Gender  
- MaritalStatus  
- Occupation  
- MonthlyIncome  
- CityTier  
- Passport  
- ProductPitched  
- DurationOfPitch  
- NumberOfFollowups  
- PitchSatisfactionScore  
- NumberOfTrips  
- PreferredPropertyStar  
- ProdTaken (Target Variable)  

- Dataset Type: Mixed (Numerical + Categorical)  
- Nature: Real-world customer dataset with missing values and inconsistencies  

---

## 🧹 Data Cleaning & Feature Engineering

The dataset required extensive preprocessing before analysis:

- Fixed inconsistent categorical values:
```python
'Fe Male' → 'Female'
```

- Removed missing values using:
```python
df.dropna()
```

- Converted discrete numerical columns into categorical/object types:
  - CityTier  
  - PreferredPropertyStar  

- Removed CustomerID column to avoid data leakage  

### 🔧 Feature Engineering
Created a new feature:
```python
TotalVisiting = NumberOfPersonVisiting + NumberOfChildrenVisiting
```

### ⚙️ Preprocessing Pipeline
- StandardScaler for numerical features  
- OneHotEncoder for categorical features  
- ColumnTransformer used for preprocessing pipeline  

---

## 📊 Exploratory Data Analysis

### 🔹 Univariate Analysis
- Customer age distribution  
- Occupation analysis  
- Product conversion distribution  

### 🔹 Bivariate Analysis
- Marital Status vs Product Purchase  
- Passport vs Product Conversion  
- Follow-Ups vs Satisfaction  

### 🔹 Multivariate Analysis
- Correlation Heatmap  
- 3D Scatter Plot  
- Customer behavior analysis across multiple features  

---

## 📌 Key Insights

### 🎯 Product Conversion
- Only 19.3% customers purchased travel packages  
- Dataset is highly imbalanced for ML modeling  

### 💍 Marital Status Analysis
- Single customers convert at 36.4%  
- Married customers convert at only 14.2%  

➡️ Singles are 2.6× more likely to buy travel packages.

### 🛂 Passport Ownership
- Passport ownership showed the highest correlation with product purchase:
```python
r = 0.271
```

→ Customers with passports are more likely to purchase travel packages.

### 📞 Pitch Effectiveness
- 3–4 follow-ups resulted in highest satisfaction and conversions  
- Excessive follow-ups reduced customer satisfaction  

### 💼 Occupation & Income
- Large business owners showed highest conversion rates  
- VP-level employees had the highest average monthly income  

### 🏙️ Travel Behaviour
- Majority of customers belonged to City Tier 1  
- Most preferred 3-star properties → budget-conscious travel behavior  

### 📈 Age Analysis
- Customers aged 30–39 were the largest customer segment  
- Older customers showed lower purchase probability  

---

## 💡 Key Learnings

- Real-world datasets often contain hidden inconsistencies  
- Small data quality issues can significantly affect analysis  
- Discrete numerical values should sometimes be treated as categorical variables  
- Customer behavior can be strongly predicted through EDA patterns  
- EDA helps businesses optimize targeting and marketing strategy  

---

## 🛠️ Tools & Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Plotly  
- Scikit-learn  


Examples:
- Conversion Rate Analysis  
- Marital Status vs Conversion  
- Correlation Heatmap  
- 3D Scatter Plot  
- Follow-Up Analysis  

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/travel-tourism-eda.git
```

### 2️⃣ Install Required Libraries
```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

### 3️⃣ Run Jupyter Notebook
```bash
jupyter notebook
```

---

## 📌 Project Status
✅ Completed  
🔄 Open for feedback and improvements  

---

## 🤝 Connect With Me
I’m currently learning Data Analytics and building real-world projects.

- LinkedIn: (https://www.linkedin.com/in/bhumika-kushwah-64ab3125a/)  
- GitHub: (https://github.com/Bhumika-kushwah)  

---

## ⭐ If You Found This Useful
Give this repository a star ⭐ and share your feedback!
