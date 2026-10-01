# EDA-Sales-Analysis-Matplotlib-Seaborn

# 📊 Sales Data Exploratory Data Analysis (EDA)

> **An Exploratory Data Analysis project using Python, Pandas, Matplotlib and Seaborn to analyze sales, profit, quantity, products, categories and city-wise performance.**

---

## 🔎 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a sales dataset containing order, date, city, category, product, sales, quantity and profit information.

The objective is to understand **sales performance, profitability, product contribution, category performance and relationships between numerical variables** using Python-based data analysis and visualization techniques.

The project demonstrates an end-to-end analytical workflow:

**Data Creation → Data Understanding → Visualization → Statistical Analysis → Correlation Analysis → Business Insights**

---

# 🎯 Business Objective

The analysis focuses on answering questions such as:

* Which product categories generate the highest sales?
* Which cities contribute the most revenue?
* Which products generate the highest sales?
* How are Sales and Profit related?
* How does Quantity relate to Sales and Profit?
* How are orders distributed across categories and cities?
* What patterns can be identified through visualization?

---

# 📂 Dataset Information

The dataset contains **20 orders and 8 columns**.

| Column     | Description                     | Data Type   |
| ---------- | ------------------------------- | ----------- |
| `Order_ID` | Unique order identifier         | Integer     |
| `Date`     | Order date                      | DateTime    |
| `City`     | City where the order was placed | Categorical |
| `Category` | Product category                | Categorical |
| `Product`  | Product name                    | Categorical |
| `Sales`    | Sales/revenue generated         | Integer     |
| `Quantity` | Number of units sold            | Integer     |
| `Profit`   | Profit generated from the order | Integer     |

### Dataset Summary

| Metric                   |     Value |
| ------------------------ | --------: |
| Total Orders             |        20 |
| Total Sales              | ₹5,21,800 |
| Total Profit             |   ₹95,000 |
| Total Quantity Sold      |        82 |
| Average Sales per Order  |   ₹26,090 |
| Average Profit per Order |    ₹4,750 |
| Cities                   |         4 |
| Categories               |         3 |
| Products                 |         9 |

---

# 🛠️ Technologies Used

| Technology          | Purpose                        |
| ------------------- | ------------------------------ |
| 🐍 Python           | Programming and analysis       |
| 🐼 Pandas           | Data manipulation and analysis |
| 🔢 NumPy            | Numerical operations           |
| 📊 Matplotlib       | Data visualization             |
| 📈 Seaborn          | Statistical visualization      |
| 📓 Jupyter Notebook | Interactive analysis           |

---

# 🔄 Project Workflow

```text
                    Sales Dataset
                         │
                         ▼
                Data Understanding
                         │
                         ▼
              Dataset Exploration
                         │
                         ▼
              Statistical Analysis
                         │
                         ▼
            Matplotlib Visualization
                         │
                         ▼
             Seaborn Visualization
                         │
                         ▼
              Correlation Analysis
                         │
                         ▼
                 Key Insights
                         │
                         ▼
              Business Understanding
```

---

# 🔍 1. Data Understanding

The dataset was first explored to understand its structure and characteristics.

### Analysis Performed

* Checked dataset shape
* Inspected column names
* Checked data types
* Examined descriptive statistics
* Counted orders by category
* Counted orders by city
* Reviewed Sales, Quantity and Profit distributions

### Dataset Shape

```text
Rows    : 20
Columns : 8
```

All 20 records contain values for the available columns in the notebook dataset.

---

# 📊 2. Sales Analysis

The total sales generated across all 20 orders are:

## 💰 ₹5,21,800

The analysis shows significant differences in sales contribution across product categories.

### Sales by Category

| Category    |         Sales |
| ----------- | ------------: |
| Electronics |     ₹3,44,500 |
| Furniture   |     ₹1,53,000 |
| Clothing    |       ₹24,300 |
| **Total**   | **₹5,21,800** |

### Key Observation

**Electronics generated the highest sales contribution among the three categories.**

---

# 💰 3. Profit Analysis

The total profit generated from the dataset is:

## 💵 ₹95,000

### Profit by Category

| Category    |      Profit |
| ----------- | ----------: |
| Electronics |     ₹60,200 |
| Furniture   |     ₹28,700 |
| Clothing    |      ₹6,100 |
| **Total**   | **₹95,000** |

### Key Observation

Electronics generated the highest total profit in the dataset, followed by Furniture and Clothing.

---

# 🏙️ 4. City-wise Analysis

The dataset contains orders from four cities:

* Delhi
* Mumbai
* Indore
* Pune

### Sales by City

| City      |         Sales |      Profit |
| --------- | ------------: | ----------: |
| Delhi     |     ₹1,70,000 |     ₹29,400 |
| Mumbai    |     ₹1,63,500 |     ₹30,350 |
| Indore    |     ₹1,13,300 |     ₹20,650 |
| Pune      |       ₹75,000 |     ₹14,600 |
| **Total** | **₹5,21,800** | **₹95,000** |

### Key Observation

Delhi generated the highest total sales, while Mumbai generated slightly higher profit than Delhi in this dataset.

---

# 🛍️ 5. Product-wise Sales Analysis

Product-level analysis was performed to identify products contributing most to total sales.

| Product    |     Sales |
| ---------- | --------: |
| Laptop     | ₹2,36,000 |
| Mobile     |   ₹97,000 |
| Sofa       |   ₹73,000 |
| Table      |   ₹46,000 |
| Chair      |   ₹34,000 |
| Headphones |   ₹11,500 |
| Shoes      |    ₹9,300 |
| T-Shirt    |    ₹8,300 |
| Jeans      |    ₹6,700 |

### Key Observation

**Laptop generated the highest sales among all products in the dataset.**

---

# 📈 6. Data Visualization

The project uses both **Matplotlib and Seaborn** to visually explore the dataset.

### Matplotlib Visualizations

The notebook includes:

* Line Plot
* Multiple Line Plot
* Bar Chart
* Horizontal Bar Chart
* Pie Chart
* Histogram
* Scatter Plot

### Seaborn Visualizations

The notebook includes:

* Line Plot
* Bar Plot
* Count Plot
* Scatter Plot
* Scatter Plot with `hue`
* Scatter Plot with `hue` and `size`
* Regression Plot
* Correlation Heatmap

---

# 🔗 7. Correlation Analysis

Correlation analysis was performed to understand relationships between:

* Sales
* Quantity
* Profit

### Correlation Matrix

| Variable     |     Sales | Quantity |    Profit |
| ------------ | --------: | -------: | --------: |
| **Sales**    |     1.000 |   -0.743 | **0.996** |
| **Quantity** |    -0.743 |    1.000 |    -0.750 |
| **Profit**   | **0.996** |   -0.750 |     1.000 |

### Important Observation

The dataset shows a **very strong positive correlation between Sales and Profit (0.996)**.

This means that, within this dataset, higher sales values are closely associated with higher profit values.

The relationship should be interpreted as an observation from this dataset and **not as proof that sales alone cause profit to increase**.

---

# 📊 8. Sales vs Profit Analysis

A scatter plot and regression plot were used to examine the relationship between Sales and Profit.

The analysis shows a strong positive relationship between the two variables.

```text
Higher Sales
     │
     │       ●
     │    ●
     │  ●
     │ ●
     └──────────────────
             Profit
```

The correlation coefficient between Sales and Profit is approximately:

```text
0.996
```

---

# 💡 Key Business Insights

Based on the analysis performed in this project:

### 1️⃣ Electronics is the major sales contributor

Electronics generated **₹3,44,500**, making it the largest contributor to total sales.

### 2️⃣ Electronics also generated the highest profit

The Electronics category generated **₹60,200 profit**.

### 3️⃣ Laptop is the highest-selling product

Laptop sales reached **₹2,36,000**, the highest among the products analyzed.

### 4️⃣ Delhi generated the highest sales

Delhi contributed **₹1,70,000 in sales**.

### 5️⃣ Mumbai generated the highest city-level profit

Mumbai generated **₹30,350 profit**, slightly above Delhi's ₹29,400.

### 6️⃣ Sales and Profit have a strong positive relationship

The correlation between Sales and Profit is approximately **0.996**, indicating a very strong positive association in this dataset.

---

# 💼 Business Value

This project demonstrates how exploratory analysis can help businesses understand their sales performance.

The analysis can support:

| Business Area             | Potential Use                                  |
| ------------------------- | ---------------------------------------------- |
| 📊 Sales Strategy         | Identify high-performing categories            |
| 🛍️ Product Strategy      | Identify products contributing most to revenue |
| 🏙️ Regional Analysis     | Compare city-level performance                 |
| 💰 Profitability          | Understand revenue-profit relationships        |
| 📈 Performance Monitoring | Track sales and profit patterns                |
| 🎯 Decision Making        | Support data-driven business decisions         |

---

# 🧠 Skills Demonstrated

### Technical Skills

```text
Python
Pandas
NumPy
Matplotlib
Seaborn
Data Analysis
Data Visualization
Statistical Analysis
Correlation Analysis
```

### Analytical Skills

```text
Data Understanding
Pattern Identification
Trend Analysis
Business Insight Generation
Data Interpretation
Problem Solving
```

---

# 📁 Repository Structure

```text
EDA-Sales-Analysis/
│
├── 📓 EDA_Sales_Analysis.ipynb
│
├── 📄 README.md
│
└── 📄 requirements.txt
```

---

# 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/EDA-Sales-Analysis.git
```

### 2. Open the project folder

```bash
cd EDA-Sales-Analysis
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
EDA_Sales_Analysis.ipynb
```

---

# 📦 Requirements

```text
pandas
numpy
matplotlib
seaborn
jupyter
```

---

# 🎓 Learning Outcomes

Through this project, I gained practical experience in:

* Understanding structured datasets
* Performing exploratory data analysis
* Using Pandas for data analysis
* Creating professional data visualizations
* Comparing category and city performance
* Analyzing product-level sales
* Understanding correlation
* Interpreting Sales vs Profit relationships
* Converting analytical results into business insights

---

# 👩‍💻 About the Project

This project is part of my **Data Science learning journey** and demonstrates my hands-on experience with Python-based data analysis and visualization.

The project follows a practical approach of:

> **Data → Analysis → Visualization → Insights → Business Understanding**

---

# ⭐ Project Highlights

```text
✔ 20 Sales Orders
✔ 8 Data Attributes
✔ Sales & Profit Analysis
✔ Category-wise Analysis
✔ City-wise Analysis
✔ Product-wise Analysis
✔ Matplotlib Visualizations
✔ Seaborn Visualizations
✔ Correlation Analysis
✔ Sales vs Profit Analysis
✔ Business Insights
```

---

## 📬 Connect With Me

**Email** durgadwivedi143@gmail.com

---

## ⭐ If You Find This Project Useful

If you found this project interesting, please consider giving the repository a ⭐.
