# **Titanic EDA in Power BI - README**

## **📌 Project Overview**
This repository contains a **complete Power BI implementation** of Exploratory Data Analysis (EDA) for the Titanic dataset. The project demonstrates:
- Data cleaning and transformation in Power Query
- Interactive visualizations and dashboards
- Advanced Power BI features (conditional formatting, slicers, tooltips)
- Export and sharing options

## **🛠️ Tools Used**
- **Power BI Desktop** (Latest Version)
- **Titanic Dataset** (from Kaggle)
- **Power Query Editor** (for data cleaning)
- **Power BI Service** (Optional - for cloud sharing)

---

## **📂 Files Included**
| File | Description |
|------|-------------|
| `Titanic_EDA.pbix` | Main Power BI report file |
| `train.csv` | Source dataset (Titanic passenger data) |
| `Titanic_EDA.pdf` | Exported PDF report (sample) |
| `README.md` | This documentation file |

---

## **🚀 Getting Started**
### **1. Prerequisites**
- Download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/)
- Download the Titanic dataset from [Kaggle](https://www.kaggle.com/c/titanic/data)

### **2. Setup Instructions**
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/titanic-powerbi-eda.git
   ```
2. Open `Titanic_EDA.pbix` in Power BI Desktop
3. If prompted about data source, update the path to `train.csv` in your local directory

---

## **🔍 Project Walkthrough**
### **Key Steps Performed**
1. **Data Cleaning** (Power Query Editor)
   - Handling missing values in Age/Cabin
   - Feature engineering (FamilySize, Title extraction)
   
2. **Visualizations**
   - Survival rate by gender/class
   - Age distribution histograms
   - Correlation heatmaps
   - Interactive scatter plots

3. **Dashboard Features**
   - Cross-filtering slicers (Pclass, Embarked, Sex)
   - Conditional formatting
   - Tooltips with passenger details

4. **Export Options**
   - PDF/PPT for static reports
   - Power BI Service for cloud sharing
   - Excel for raw data export

---

## **📊 Key Insights Discovered**
- **74% of females survived** vs only 19% of males
- **1st class passengers had 63% survival rate** (vs 24% in 3rd class)
- Children under 10 had higher survival chances
- Higher fare correlated with better survival odds

---

## **💡 How to Customize**
1. **Modify Visuals**:
   - Right-click any visual → "Edit" to change chart types
   - Adjust colors in Format pane

2. **Add New Data**:
   - Click "Transform Data" to modify Power Query steps
   - Add `test.csv` for extended analysis

3. **Create Calculated Measures**:
   ```DAX
   Survival Rate = DIVIDE(SUM(Titanic[Survived]), COUNTROWS(Titanic), 0)
   ```

---

## **📚 Resources**
- [Power BI Documentation](https://learn.microsoft.com/en-us/power-bi/)
- [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- [Power BI Community Forum](https://community.powerbi.com/)

---

**🌟 Please star this repo if you found it useful!**  
[![GitHub Stars](https://img.shields.io/github/stars/navyasri-143/titanic-powerbi-eda?style=social)](https://github.com/yourusername/titanic-powerbi-eda)
