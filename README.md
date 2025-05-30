
# 🚗 Automobile Sales Data Analysis & Dashboard

![Dashboard Preview](![RecessionReportgraphs png](https://github.com/user-attachments/assets/167304f5-4b67-46da-b7c1-6e4381a67b5c))

This project is my final assignment for the IBM Data Visualization course. I analyzed historical automobile sales data using Python and created an interactive dashboard using Dash. The project is split into two parts:

- **Part 1**: Data analysis and visualization in a Jupyter Notebook.
- **Part 2**: Interactive dashboard built with Dash.

---

## 📁 Project Files

- `DV0101EN-Final-Assign-Part1.ipynb`: Jupyter Notebook for data analysis and visualizations.
- `DV0101EN-Final-Assign-Part-2-Questions.py`: Dash app script for building the interactive dashboard.
- `dashboard_screenshot.png`: Dashboard preview image.

---

## 🎯 Objective

To explore and visualize historical automobile sales data with a focus on:
- Recession vs non-recession periods
- Sales trends over years and months
- Vehicle type performance
- Advertising expenditure patterns
- Effect of unemployment on sales

---

## 🛠 Tools and Libraries Used

- **Python**
- **Pandas** – data manipulation
- **Plotly** – visualization library
- **Dash** – web app framework
- **Jupyter Notebook** – exploratory analysis

---

## 📊 Part 1 – Notebook Analysis: Detailed Tasks and Insights

### ✅ Task 1: Import Data and Libraries
**What I Did**: Loaded the CSV dataset using `pandas.read_csv()` and imported libraries like Plotly and Seaborn for visualization.

**Insight**: Verified data structure and ensured the necessary columns were present: Year, Month, Recession, Automobile_Sales, Vehicle_Type, Advertising_Expenditure, Unemployment Rate.

---

### ✅ Task 2: Filter Data for Recession Periods
**What I Did**: Used `df[df['Recession'] == 1]` to isolate data for recession years.

**Insight**: Focused only on recession periods to observe specific economic impacts on vehicle sales.

---

### ✅ Task 3: Average Sales During Recession by Year
**What I Did**: Grouped by Year and calculated average automobile sales using `groupby()`.

**Visualization**: Line chart

**Insight**: Sales dropped significantly during recession years, highlighting economic sensitivity.

---

### ✅ Task 4: Average Sales by Vehicle Type During Recession
**What I Did**: Grouped data by Vehicle_Type to compute average sales.

**Visualization**: Bar chart

**Insight**: Cars and SUVs were the most sold vehicles even during recessions.

---

### ✅ Task 5: Advertising Expenditure During Recession
**What I Did**: Grouped by Vehicle_Type and summed the advertising expenditure.

**Visualization**: Pie chart

**Insight**: Cars received the most ad budget, even during tough times.

---

### ✅ Task 6: Effect of Unemployment Rate During Recession
**What I Did**: Grouped by Unemployment Rate and Vehicle Type to compare average sales.

**Visualization**: Bar chart

**Insight**: Higher unemployment correlated with lower vehicle sales, especially for non-essential types.

---

### ✅ Task 7: Yearly Automobile Sales Trend
**What I Did**: Calculated average sales across all years.

**Insight**: Sales fluctuate with economic conditions, with obvious dips during recessions.

---

### ✅ Task 8: Monthly Sales Pattern
**What I Did**: Grouped by Month to see which months had higher/lower sales.

**Insight**: Some months like June/December often perform better due to promotions or seasonal trends.

---

## 📈 Part 2 – Dash App: Interactive Dashboard Tasks

### ✅ Task 2.1: Add Title to Dashboard
Set the dashboard title: **"Automobile Sales Statistics Dashboard"** using `html.H1()`.

---

### ✅ Task 2.2: Add Dropdowns for Statistics and Year
Two dropdowns created:
- One for choosing "Recession Period Statistics" or "Yearly Statistics"
- One for selecting a year (enabled only for "Yearly Statistics")

---

### ✅ Task 2.3: Display Output Container
Created an output container to show graphs dynamically based on dropdown selection.

---

### ✅ Task 2.4: Enable/Disable Year Dropdown Based on Selection
**What I Did**: Used Dash `@app.callback` to enable year dropdown only when "Yearly Statistics" is selected.

---

### ✅ Task 2.5: Create Recession Graphs
- Line chart for average sales during recession
- Bar chart of average sales by vehicle type
- Pie chart of ad expenditure during recession
- Bar chart showing unemployment vs sales

**Insight**: Confirmed recession period analysis from the notebook using interactive charts.

---

### ✅ Task 2.6: Create Yearly Graphs
- Line chart for yearly trend
- Line chart for monthly pattern
- Bar chart for vehicle sales by type (in selected year)
- Pie chart for ad expenditure by type (in selected year)

**Insight**: Enables users to explore year-specific data and patterns.

---

## ▶️ How to Run the Dashboard

1. Install dependencies:
```bash
pip install dash pandas plotly
```

2. Run the script:
```bash
python DV0101EN-Final-Assign-Part-2-Questions.py
```

3. Open browser and go to:
```
http://127.0.0.1:8050/
```

---

## 📌 Conclusion

Through this project, I explored how automobile sales are affected by different factors like economic conditions, advertising, and unemployment. By building both a static analysis and an interactive dashboard, I learned:

- How to clean and explore real-world data
- How to visualize trends and derive business insights
- How to use Dash to create a responsive, interactive dashboard
- How different metrics like unemployment and advertising influence automobile sales

This project helped me practice both data analytics and visualization, and create something I can share on my GitHub portfolio.

---

## 👩‍💻 Author

**Manisha Linguntla**
