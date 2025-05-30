# 🚗 Automobile Sales Data Analysis & Dashboard

![Dashboard Preview](dashboard_screenshot.png)

This is my final assignment project for the IBM Data Visualization course. I used Python to analyze historical automobile sales data and created visualizations. I also built an interactive dashboard using Dash to explore the data easily.

---

## 📁 Project Files

- `DV0101EN-Final-Assign-Part1.ipynb`: A Jupyter Notebook where I explored and visualized the data.
- `DV0101EN-Final-Assign-Part-2-Questions.py`: A Dash app that creates an interactive dashboard to explore the data further.

---

## 📌 Project Goal

The main goal is to understand how automobile sales have changed over time, especially during recession periods. I also looked at how different vehicle types performed, how much was spent on advertising, and how unemployment affected sales.

---

## 🛠 Tools and Libraries Used

- **Python**
- **Pandas** – for working with the data  
- **Plotly** – for creating beautiful charts  
- **Dash** – to build the interactive web dashboard  
- **Jupyter Notebook** – for analysis and static graphs

---

## 📊 What I Did in Part 1 (Notebook)

### Steps I Followed:

- Loaded and cleaned the data using pandas.
- Analyzed the difference between recession and non-recession periods.
- Grouped the data by year, month, and vehicle type.
- Created line charts, bar charts, and pie charts using Plotly.

### ✅ My Findings:

- Sales were lower during recession years.
- Cars and SUVs had higher sales than other vehicle types.
- Companies spent more on advertising for cars and SUVs.
- When unemployment was high, car sales went down.

---

## 📈 What I Did in Part 2 (Dashboard)

### Features of the Dashboard:

- Has dropdowns to select:
  - **Yearly Statistics**
  - **Recession Period Statistics**
- Shows multiple visualizations:
  - Yearly and Monthly Sales Trends
  - Vehicle Type Sales
  - Advertising Spend by Vehicle
  - Impact of Unemployment on Sales

### How to Run This Dashboard:

1. Make sure these libraries are installed:
   ```bash
   pip install dash pandas plotly
