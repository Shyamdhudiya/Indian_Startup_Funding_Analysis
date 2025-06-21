# 💡 Data Analysis on Indian Startup Funding (2018–2021)

<img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*I0pbJXG4v0fGGUlxAYIOng.jpeg" width="550">

## 📌 Project Overview

This project explores Indian startup funding trends from 2018 to 2021 using multiple datasets. The objective is to clean, analyze, and visualize funding patterns based on various factors like company, sector, location, and funding amount to derive business insights.

---

## 📁 Dataset Information

The data was collected from four CSV files:
- `startup_funding2018.csv`
- `startup_funding2019.csv`
- `startup_funding2020.csv`
- `startup_funding2021.csv`

Each dataset contains information about:
- Company/Brand
- Sector
- Stage of funding
- Amount funded
- Headquarter location
- Founders
- Investor
- Founded year

---

## 🧹 Data Cleaning

The following steps were taken to clean and preprocess the data:
- **Renamed columns** to maintain consistency across years.
- **Removed unnecessary columns** like `Unnamed: 9`.
- **Added missing columns** to ensure uniform structure.
- **Handled currency inconsistencies**, converting all amounts to USD and removing non-numeric characters.
- **Imputed missing values** using:
  - Mean for numerical (`Amount($)`)
  - Mode for categorical (e.g., `Sector`, `Stage`)
- **Standardized categorical values** (e.g., unified spelling for "E-commerce").
- **Removed duplicates**.

---

## 📊 Exploratory Data Analysis

### Questions Answered:

1. **Which companies received the most funding?**
2. **Which locations received the least funding?**
3. **Which sectors received the most investment?**
4. **How much was contributed by investors in Delhi and Mumbai?**

### Visualizations:
- Bar plots (top companies, sectors, cities)
- Pie charts (Stage distribution)
- KDE plots and Histograms
- Correlation Heatmap
- Scatter plots and regression analysis

---

## 📐 Feature Engineering

- Used **MinMaxScaler** for scaling `Founded` and `Amount($)` columns.
- Applied **One-Hot Encoding** for categorical variables:
  - Company/Brand
  - Sector
  - Stage
  - HeadQuarter
  - What it does
  - Founders
  - Investor

---

## 🔍 Tools & Libraries

- **Python** (Jupyter/Colab)
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 📈 Key Insights

- Some companies dominate the funding landscape.
- Certain cities and sectors consistently attract high investments.
- Clear funding trends are seen across different stages and years.

---

## 📎 Project Files

- `data_analysis_on_indian_startup_funding.py`: Main Python script
- `startup_funding2018.csv` to `2021.csv`: Datasets used

---

## 🙋‍♂️ Author

**Shyam Dhudiya**

- 📧 Email: dhudiyashyam84@gmail.com  
- 💼 LinkedIn: [linkedin.com/in/shyam-dhudiya-75240b302](https://linkedin.com/in/shyam-dhudiya-75240b302)

---

## 🏁 Future Work

- Predictive modeling to estimate future funding trends
- NLP-based analysis of company descriptions
- Dashboard integration using Power BI or Tableau

---

## ⭐ How to Use

1. Clone the repo or upload script on Colab.
2. Upload all four CSV files.
3. Run all cells to see analysis & visualizations.
4. Explore encoded and scaled data for further modeling.

---

## 📜 License

This project is open-source and available under the MIT License.
