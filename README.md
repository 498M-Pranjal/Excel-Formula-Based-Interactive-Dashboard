# Excel-Sales-Dashboard-CY-vs-PY

**Project Overview**

This Excel Sales Dashboard compares product-wise and month-wise sales of the Current Year (CY) with the Previous Year (PY). 
It helps analyze YoY growth, target vs actual performance, and sales trends using dynamic filters and charts.

**Objective**

* Compare CY vs PY sales month-wise

* Calculate YoY % Change

* Track target sales

* Create a clean and interactive Excel dashboard using formulas

**Dataset (Input) vs Dashboard (Output):**

**Dataset (Input):**

Raw transactional sales data containing:

* Order Date

* Product Category

* Sales Amount

**Dashboard (Output):**

* Month-wise CY Sales

* Month-wise PY Sales

* YoY % Change

* Target Sales comparison

* Interactive charts and indicators

**Dashboard Controls:**

* Year Selector (Dropdown using Data Validation)

* Product Selector (e.g., Mountain Bikes)

* Dynamic update of all tables and charts based on selection

**Dashboard Components:**

🔹 **KPI Section**

* Annual Sales (CY)

* % Contribution to Total Sales

* Total Sales (All Products)

**🔹 Monthly Comparison Table**

* Month

* CY Sales

* PY Sales

* YoY % Change

* Conditional Formatting with Data Bars

**🔹 Charts**

* Line Chart showing:

 * CY Sales

 * PY Sales

 * Target Sales (Dashed Line)

* Smoothed lines for better trend visibility

* Proper legends and labels

**1. Dataset (Input) vs Dashboard (Output)**

Raw data is transformed into a visual dashboard using formulas and charts.

**2️. Overview of Formulas Used**

* SUMIFS

* INDEX

* MATCH

* IFERROR

* YEAR

* TEXT

* VLOOKUP

* Logical Functions (AND, OR, NOT)

* Aggregate calculations

**3️. Symbols (Arial)**

Icons and symbols are used for visual indicators using the Arial font.

**4️. Drop-down List using Data Validation**

Used for:

* Year selection

* Product selection

**5️. SUMIFS using Multiple Criteria**

Sales calculated based on:

* Year

* Product

* Month

**6️. Using YEAR & TEXT**

* YEAR() to extract year from date

* TEXT() to format months

**7️. YoY % Change**

Calculated to compare CY vs PY performance.

**8️. Conditional Formatting – Data Bars**

* Axis at cell midpoint

* Show bar only

* Red/Blue indicators for decrease/increase

**9️. INDEX + MATCH with Wildcards**

* (asterisk) *

* ~ (tilde)
  
Used for flexible product matching.

**10. Line Chart Customization**

* Dashed line for target sales

* Smoothed line enabled

* Series name as data label

**11. Final Touches**

* Dark theme formatting

* Alignment & spacing

* Professional dashboard look

**Key Excel Formulas Used**

**🔹 CY Sales**

CY Sales = SUMIFS(Sales_Range, Year_Range, Selected_Year, Product_Range, Selected_Product, Month_Range, Selected_Month)

**🔹 PY Sales**

PY Sales = SUMIFS(Sales_Range, Year_Range, Selected_Year-1, Product_Range, Selected_Product, Month_Range, Selected_Month)

**🔹 YoY % Change**

YOY % Change = IFERROR((CY_Sales - PY_Sales) / PY_Sales, 0)

**🔹 INDEX MATCH with Wildcard**

Index match = INDEX(range, MATCH("*"&lookup_value&"*", lookup_range, 0))

**Features Used**

* Data Validation

* Conditional Formatting

* Logic Operators

* Aggregate Functions

* Lookup Functions

**Conclusion**

This Excel Sales Dashboard provides a powerful way to analyze monthly and product-wise sales performance using formulas and charts.
It demonstrates a strong understanding of Excel analytics, business logic, and dashboard design.

**Dashboard Screenshot:**

<img width="1837" height="693" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/0ab637e5-04a5-402c-828b-c141d78d53f1" />

