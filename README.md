# 🚗 Automobile Sales Data Analysis & Dashboard

![RecessionReportgraphs png](https://github.com/user-attachments/assets/3476a799-68c5-44a2-b9a7-0ee387e8bc43)


![YearlyReportgraphs png](https://github.com/user-attachments/assets/5b9dfd46-12e9-45a1-bb87-6a96b1fdc7e6)


This project is my final assignment for the IBM Data Visualization course. I analyzed historical automobile sales data using Python and created an interactive dashboard using Dash. The goal was to explore how automobile sales change during recession and non-recession periods, identify trends, and visualize the impact of external factors like advertising and unemployment.

The project has two parts:

- **Part 1**: Data analysis and static visualizations using Jupyter Notebook.
- **Part 2**: Interactive dashboard using Dash and Plotly.

---

## 📁 Files Included

- `DV0101EN-Final-Assign-Part1.ipynb`: Analysis and plots in Jupyter Notebook  
- `DV0101EN-Final-Assign-Part-2-Questions.py`: Dash app code  

---

## 🛠 Tools Used

- Python  
- Pandas  
- Seaborn, Matplotlib, Plotly  
- Dash (for dashboard UI)  
- Jupyter Notebook  

---

## 📊 Part 1 – Jupyter Notebook: Tasks, Charts, and Insights

### 🧪 TASK 1.1: Line Chart – Yearly Automobile Sales Trend
- **What I Did**: Grouped the data by year and calculated average automobile sales using Pandas.
- **Chart**: Line plot showing yearly trend.

![Line_Plot_1 png](https://github.com/user-attachments/assets/3a364113-9a5c-49e4-b5fb-fe606da526fa)

- **Insight**: Sales dropped in recession years and picked up in recovery periods.

---

### 🚗 TASK 1.2: Line Chart – Sales by Vehicle Type During Recession
- **What I Did**: Filtered recession years and plotted sales trends for each vehicle type.
- **Chart**: Multiple line plots by vehicle type.

  ![Line_Plot_2 png](https://github.com/user-attachments/assets/c4b89c34-ed94-420f-a253-0c5fc9b92d24)

- **Insight**: Cars and SUVs performed better; executive and sports cars dropped significantly.

---

### 📉 TASK 1.3: Seaborn Plot – Compare the sales trend per vehicle type for a recession period with a non-recession period.
- **What I Did**: Compared vehicle type sales using Seaborn for both recession and normal years.
- **Chart**: Bar chart.

  ![Screenshot 2025-05-29 182542](https://github.com/user-attachments/assets/00850222-554e-41b9-84cd-6a5d6d0bd176)

  ![Bar_Chart png](https://github.com/user-attachments/assets/08d91ba8-62c4-43ac-9ae5-6fa870fdd5f4)

- **Insight**: Overall drop in sales during recession; family and economy vehicles stayed more stable.

---

### 💹 TASK 1.4: Subplots – GDP Trend Comparison
- **What I Did**: Used Matplotlib subplots to compare GDP during recession and non-recession years.
- **Chart**: Two line plots (side-by-side).

  ![Subplot png](https://github.com/user-attachments/assets/9f4eb938-f040-4a14-be3e-4978864de3eb)

- **Insight**: GDP was consistently lower during recession periods.

---

### 🟠 TASK 1.5: Bubble Chart – Seasonality Impact
- **What I Did**: Plotted bubble size by seasonality weight, with months and sales on the axes.
- **Chart**: Bubble chart using Plotly.

  ![Bubble png](https://github.com/user-attachments/assets/4b020f92-62a1-4ae5-91f2-0aa03f4673b5)

- **Insight**: June and December had the highest seasonal sales impact.

---

### 📊 TASK 1.6: Scatter Plots – Price & Confidence vs Sales
- **What I Did**: Created scatter plots for:
  - Average price vs automobile sales
  - Consumer confidence vs sales during recession
- **Chart**: Two scatter plots.


![Screenshot 2025-05-29 212519](https://github.com/user-attachments/assets/e2910632-9622-4ca6-9b03-11304a0ec085)

![Scatter png](https://github.com/user-attachments/assets/ef283db3-75f8-4253-892d-b293560aaa78)

- **Insight**: Higher prices reduce sales; low consumer confidence strongly correlates with low sales.

---

### 🧾 TASK 1.7: Pie Chart – Ad Expenditure During Recession vs Normal Periods
- **What I Did**: Compared total ad spending grouped by recession flag.
- **Chart**: Pie chart.

![Pie_1 png](https://github.com/user-attachments/assets/4b355a72-6a3a-499c-9e71-28e2ffaf309e)

- **Insight**: Ad spending slightly dropped in recessions but was still significant.

---

### 🚘 TASK 1.8: Pie Chart – Ad Spend by Vehicle Type During Recession
- **What I Did**: Grouped ad expenditure by vehicle type.
- **Chart**: Pie chart for recession period only.

  ![Pie_2 png](https://github.com/user-attachments/assets/fb332a87-5c9f-4e28-a2a1-11ef4f2089e4)

- **Insight**: Cars and SUVs got the majority of the ad budget.

---

### 📉 TASK 1.9: Line Plot – Unemployment Rate Impact on Vehicle Type and Sales During Recession
- **What I Did**: I filtered the dataset to include only recession periods (`Recession = 1`). Then, I grouped the data by `Unemployment_Rate` and `Vehicle_Type`, and calculated the average `Automobile_Sales` for each group.
- **Chart**: Line plot (or bar chart) showing how unemployment rate affects average sales for each vehicle type.
  ![Line_Plot_3 png](https://github.com/user-attachments/assets/740cf91e-2bf7-411c-812d-48d59adbb49d)

- **How I Did It**:
  - Used `groupby(['Unemployment_Rate', 'Vehicle_Type'])['Automobile_Sales'].mean().reset_index()` to prepare the data.
  - Plotted the results using `plotly.express` with `x='Unemployment_Rate'`, `y='Automobile_Sales'`, and `color='Vehicle_Type'` for multiple lines or bars.
- **Insight**: As unemployment increased, average automobile sales decreased across all vehicle types. Premium and luxury vehicles saw sharper drops, showing that consumers reduced spending on non-essential vehicles during uncertain times.

---

## 📈 Part 2 – Dash App: Tasks, Charts, and Functionality

### 🎯 TASK 2.1: Title
- Set the dashboard title: **"Automobile Sales Statistics Dashboard"**.
![Title png](https://github.com/user-attachments/assets/830c9b1e-7585-4101-b464-9b70921bd65b)

---

### 🎛 TASK 2.2: Dropdown Menus
- **1st Dropdown**: Choose either Recession Period Statistics or Yearly Statistics.
- **2nd Dropdown**: Select a specific year (enabled only if "Yearly Statistics" is selected).
![Dropdown png](https://github.com/user-attachments/assets/8c508bd1-0d5e-4306-acd0-60bcbdbbdafd)

---

### 📤 TASK 2.3: Output Container
- Created a div element to display all generated charts dynamically.
![Outputdiv png](https://github.com/user-attachments/assets/c3624574-dd84-4bbe-9be5-1c8e20571d92)

---

### 🧠 TASK 2.4: Callback to Enable/Disable Year Dropdown
- Used Dash’s callback to disable the year selector if "Recession Period Statistics" is selected.
![Callbacks png](https://github.com/user-attachments/assets/ab7278f6-6de8-403f-b6a3-00a13efb1f9a)

---

### 📊 TASK 2.5: Recession Statistics Graphs
When "Recession Period Statistics" is selected:
- **Chart 1**: Line chart – Average sales by year during recession.
- **Chart 2**: Bar chart – Average sales by vehicle type.
- **Chart 3**: Pie chart – Ad expenditure share by vehicle type.
- **Chart 4**: Bar chart – Unemployment rate vs sales.
![RecessionReportgraphs png](https://github.com/user-attachments/assets/910a677c-5299-4e05-9cdd-9f9512941eb6)

---

### 📅 TASK 2.6: Yearly Statistics Graphs
When a specific year is selected:
- **Chart 1**: Line chart – Sales trend over years.
- **Chart 2**: Line chart – Monthly average sales.
- **Chart 3**: Bar chart – Avg. vehicles sold in the selected year.
- **Chart 4**: Pie chart – Ad spend by vehicle type.
![YearlyReportgraphs png](https://github.com/user-attachments/assets/92b86b20-570f-4e88-aa02-b850f3367c4d)

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

Through this project, I explored how automobile sales are affected by different factors like economic conditions, advertising, and unemployment. This project helped me apply data analysis and visualization techniques to understand the impact of economic factors on automobile sales. By comparing recession and non-recession periods. By building both a static analysis and an interactive dashboard, I learned:

- Recession years consistently show lower sales, especially for luxury vehicle types.
- Consumer confidence and unemployment are directly linked to sales performance.
- Advertisement spending remained high even during tough times, especially for cars and SUVs.
- Seasonality plays a key role in driving monthly sales patterns.
- I also learned how to build an interactive dashboard using Dash, giving users the ability to explore insights easily.
This project helped me practice both data analytics and visualization, and create something I can share on my GitHub portfolio.

---

## 👩‍💻 Author

**Manisha Linguntla**

