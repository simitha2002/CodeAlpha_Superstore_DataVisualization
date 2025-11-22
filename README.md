# 📊 Superstore Dataset – Data Visualization

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Status](https://img.shields.io/badge/Status-Complete-success.svg)
![CodeAlpha](https://img.shields.io/badge/CodeAlpha-Internship-orange.svg)

**CodeAlpha Data Analytics Internship - Task 3: Data Visualization**

![Banner](banner.png)
---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Data Preparation & Feature Engineering](#Data-Preparation-&-Feature-Engineering)
- [Visualizations](#Visualizations)
- [Key Insights](#key-insights)
- [Recommendations](#Recommendations)
- [Challenges & Solutions](#challenges--solutions)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [Contact](#contact)

---

## 🎯 Overview

This project focuses on **Data Visualization** using the popular **Superstore Dataset**, as part of the **CodeAlpha Data Analytics Internship (Task 3)**.

The notebook performs:

- Data cleaning
- Feature engineering
- Aggregations
- Visual analysis of sales, profit, categories, regions, shipping, and customer behavior

The goal is to transform raw retail data into **clear, meaningful visual insights** that support business decision-making.

---

## ✨ Features

### 🧹 Data Preparation
- Converted date fields using `parse_dates`
- Removed duplicates
- Cleaned invalid shipping times
- Created new features: **Year, Month, Month_Name, No_of_days (Shipping time), Cost, Profit_rate**

### 📊 Visualization
Includes detailed charts for:

- Monthly sales trends
- Category & sub-category performance
- Region-wise revenue
- Top customers
- Distribution of sales, profit, cost, quantity, profit rate
- Scatter plots: Profit vs Sales, Profit Rate vs Discount
- Correlation heatmap
- Shipping time distribution
- Profit summary visualization

---

## 💻 Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Python 3.8+** | Core programming language |
| **Pandas** | Data manipulation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Advanced visual analytics |
| **Jupyter Notebook** | Interactive development environment |

---

## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Jupyter Notebook

### Step 1: Clone the Repository
```bash
git clone https://github.com/simitha2002/CodeAlpha_Superstore_DataVisualization.git
cd CodeAlpha_Superstore_DataVisualization
```

### Step 2: Create Virtual Environment (Recommended)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python3 -m venv venv
source venv/bin/activate
```

## 📖 Usage

### Option 1: Run Jupyter Notebook
```bash
jupyter notebook notebooks/Task3.ipynb
```

Then run all cells sequentially (Cell → Run All)

### Option 2: Quick Start
```python
# Import required libraries
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

# Load cleaned data
df = pd.read_csv('data/Superstore_Cleaned.csv')

df.head()
df.describe()
```

## 📁 Project Structure
---

```
CodeAlpha_Superstore_DataVisualization/
│
├── Task3.ipynb                       # Main analysis notebook                      
│
├── data/
│   ├── Superstore.csv                # Original dataset (uncleaned)
│   └── Superstore_Cleaned.csv        # Cleaned dataset
│
├── banner.png                        # Banner image
│
└── README.md                         # Documentation
```

---

## 🧹 Data Preparation & Feature Engineering

- Parsed `Order Date` & `Ship Date`
- Removed negative shipping durations
- Removed duplicates
- Added `Year`, `Month`, `Month_Name`
- Created new feature: `TotalSales = Quantity * Price`
- Calculated `No_of_days` = Ship Date - Order Date
- Derived:
      - `Cost` = Sales - Profit
      - `Profit_rate` = Profit / Cost

---

## 📊 Visualizations
**Includes:**
- Line chart: Monthly Sales Trend
- Bar charts: Category, Region, Sub-Category, Customer Sales
- Distribution plots: Sales, Discount, Profit, Profit Rate
- Scatter plots: Profit vs Sales, Discount vs Profit Rate, Sales vs Shipping Duration
- Heatmap: Correlation matrix
- Summary: Total Sales, Gain, Loss
- Shipping Time Frequency plot

---

## 🔍 Key Insights

### 📅 Sales Trends

- Sales steadily increase from **2014 to 2017**.
- **November** consistently records the **highest** sales.
- **February–March** has the **lowest** sales each year.
  
### 🛒 Category Insights

- **Technology** has the **highest** sales revenue.
- **Office Supplies** dominates order volume.
- Top-selling sub-categories include **Phones and Chairs**.

### 🌍 Regional Insights

- **West and East** regions perform best.
- **South** region requires improvement.

### 📈 Profitability Insights

- High discounts sharply reduce profit rates.
- Furniture category shows low and unstable profitability.
- Some high-sales transactions still generate losses.

### 🚚 Shipping Insights

- Most orders take **4–5 days** to ship.
- Fast shipping (0–1 days) is rare.
- Shipping duration does not significantly affect sales.
  
---

## 💡 Recommendations
- Reduce steep discounts that lead to negative profits.
- Improve furniture profitability through pricing review.
- Prepare inventory & marketing for November peak season.
- Strengthen the South region’s sales strategy.
- Create loyalty programs for top customers.
- Increase stock for high-performing sub-categories.
- Enhance shipping speed to improve customer experience.

---

## 🚧 Challenges & Solutions

### Challenge 1: ⚠️ Negative Shipping Times
**Solution:** Replaced negative values with `NaN`.  

### Challenge 2: ⚠️ Profit Loss Outliers 
**Solution:** Analyzed discount impact and added Profit_rate feature.

### Challenge 3: ⚠️ Skewed Distributions
**Solution:** Visualized distributions and used log scales where needed. 

---

## 🔮 Future Enhancements

- [ ] Add interactive dashboard (Tableau / Power BI)
- [ ] Add forecasting model for monthly sales
- [ ] Perform customer segmentation (RFM)
- [ ] Automate daily/weekly reporting

---

## 🤝 Contributing

Contributions are welcome!
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch 
5. Open a Pull Request

---

## 📞 Contact

**Simitha Ummer**

- LinkedIn: [linkedin.com/in/simitha-ummer](http://www.linkedin.com/in/simitha-ummer-69a848350)
- GitHub: [github.com/simitha2002](https://github.com/simitha2002)
- Email: simithau@gmail.com

**Project Link:** [https://github.com/simitha2002/CodeAlpha_Superstore_DataVisualization](https://github.com/simitha2002/CodeAlpha_OnlineRetail_Analysis_EDA)

---

## 🙏 Acknowledgments

- **CodeAlpha** for the internship opportunity
- **Kaggle** for publicly available data
- **Python Community** for powerful open-source tools

---

## ⭐ Show Your Support

If you found this project helpful, please give it a ⭐️!

---
