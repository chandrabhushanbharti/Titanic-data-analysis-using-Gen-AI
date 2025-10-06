# 🧠 Data Analysis using GenAI — Titanic Dataset

### 👨‍💻 Author: **Chandrabhushan Kumar Bharti**  
 

---

## 🚀 Project Overview

This project explores the **Titanic passenger dataset** using **Generative AI (ChatGPT)** and **Python (Google Colab)**.  
It walks through the complete **data-analysis workflow** — from loading data to visualizing insights about passenger survival.

By the end, you’ll understand how **age, fare, class, and family relationships** influenced survival chances on the Titanic.

---

## 🧩 Dataset Used

**Dataset:** `titanic.csv`

### Key Columns
| Column | Description |
|---------|-------------|
| `survived` | 0 = Did not survive, 1 = Survived |
| `pclass` | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| `sex` | Gender |
| `age` | Passenger’s age |
| `sibsp` | # of siblings / spouses aboard |
| `parch` | # of parents / children aboard |
| `fare` | Ticket fare |
| `embarked` | Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## 🧭 Task Summary

### 🗂 **Task 1 — Load the Data**
Loaded the Titanic dataset into ChatGPT and Google Colab for analysis.

### 📊 **Task 2 — Basic Statistics**
Calculated **Mean, Median, Mode, Std Dev, Min, Max** for 5 important columns:  
`age`, `fare`, `pclass`, `sibsp`, `parch`.

| Column | Mean | Median | Mode | Std Dev | Min | Max |
|--------|------|--------|------|---------|-----|-----|
| age | 29.70 | 28.00 | 24.0 | 14.53 | 0.42 | 80.00 |
| fare | 32.20 | 14.45 | 8.05 | 49.69 | 0.00 | 512.33 |
| pclass | 2.31 | 3.00 | 3.00 | 0.84 | 1.00 | 3.00 |
| sibsp | 0.52 | 0.00 | 0.00 | 1.10 | 0.00 | 8.00 |
| parch | 0.38 | 0.00 | 0.00 | 0.81 | 0.00 | 6.00 |

---

### 🧹 **Task 3 — Missing Values & Outliers**
- Checked missing data per column  
- Identified outliers using the **IQR (Interquartile Range)** method  
- Replaced negative lower bounds with 0 (not realistic in this context)

**Key Observations**
- `age` had 177 missing values and a few outliers > 64.8  
- `fare` had 116 high-fare outliers  
- `pclass` had no outliers  
- `sibsp` and `parch` had many family-size outliers  

---

### 📈 **Task 4 — Univariate Analysis**
Visualized distribution and boxplots for all 5 columns.

**Insights**
- **Age:** Right-skewed; most passengers 20-40 yrs  
- **Fare:** Highly right-skewed; few very high values  
- **Pclass:** Most in 3rd class  
- **SibSp:** Majority 0 or 1  
- **Parch:** Mostly 0; few large families  

---

### 🔁 **Task 5 — Bivariate Analysis with Survival**
Compared each feature with the target `survived`.

**Key Insights**
- 🧒 **Age vs Survival:** Younger passengers, especially children, had higher survival rates  
- 💰 **Fare vs Survival:** Higher fare → better chances of survival (wealth effect)  
- 🏷 **Pclass vs Survival:** 1st class survived more often than 3rd  
- 👨‍👩‍👧‍👦 **SibSp vs Survival:** Small families (1–2 members) had better survival rates  
- 👶 **Parch vs Survival:** Passengers with 1–3 parents/children had better chances  

---

## 💻 Technologies Used
- 🐍 **Python 3**  
- 📚 **Pandas**, **NumPy**, **Seaborn**, **Matplotlib**  
- ☁️ **Google Colab**  
- 🤖 **ChatGPT (for prompt-driven data analysis)**  

---

## 🧠 What I Learned
- Cleaning, analyzing, and visualizing real-world data  
- Detecting missing values and outliers  
- Understanding relationships between features and targets  
- Writing Colab-friendly Python code for data analysis  

---

## 📂 Project Structure
📁 Data-Analysis-using-GenAI
│
├── titanic.csv # Dataset file
├── titanic_analysis.ipynb # Colab notebook with all code
├── Data Analysis using GenAI assignment.docx # Full report
└── README.md # This file



---

## ▶️ How to Run
1. Open the notebook in **Google Colab**  
2. Upload `titanic.csv`  
3. Run each cell in sequence  
4. View outputs and charts  

---

## 📊 Example Visuals
- Histograms + Boxplots for Univariate Analysis  
- Countplots and Scatterplots for Bivariate Analysis  
- Clear patterns of survival by class and fare  

---

## 🌟 Conclusion
The analysis confirms that **social and economic status** played a major role in Titanic survival.  
This project demonstrates how **Generative AI + Python** can collaborate for fast, interpretable data insights.

---

### 🏁 End of Project
> *“Data tells stories — you just need to listen carefully.”*

