# Mobilemetrics Dashboard

![Main Dashboard](https://github.com/user-attachments/assets/fe0bf9fc-dbcf-44f6-a36d-6ec0f1261d7b)

### Project Overview:

This project is a Mobile Sales Analysis Dashboard created using Power BI. It provides insights into total sales, quantity sold, customer ratings, payment methods, and city-wise sales for mobile devices. The dashboard is designed for business analysis and decision-making purposes, giving a comprehensive view of sales performance over months and across various dimensions.

### Dataset Information:
The dataset includes fields such as Date, City, Brand, Mobile Model, Sales Amount, Quantity Sold, Customer Ratings, and Payment Method.

### Data Cleaning Performed

- Standardized number formats.

- Checked for duplicates and null values.

- Corrected decimal values

### Custom Columns and Measures Added:

- Date (Custom Column)

    Step 1. Transform Data
  
    Step 2. AddColumn Tab
  
    Step 3. Custom Column
  
    Step 4. New Column names
  
    Step 5. Formula (=[Day]&"-"&[Month]&"-"[Year])
  
    Step 6. click OK

    Step 7. Close & Apply

- Average

    Average = AVERAGE(Sales_Data[Price Per Unit])

- Top City

    Top_City = CALCULATE(MAX(Sales_Data[City]),FILTER(Sales_Data, Sales_Data[Price Per Unit]) = MAX(Sales_Data[Price Per Unit]))

- Top Quantity

    Total_Quantity = SUM(Sales_Data[Units Sold])

- Total Sales

    Total_Sales = SUMX(Sales_Data, Sales_Data[Units Sold] * Sales_Data[Price Per Unit])

- Total Transactions

    Transactions = COUNTROWS(Sales_Data)

### Key Insights:

- Delhi had the highest total sales among cities.

- Apple and Samsung brands dominated the sales figures.

- UPI and Debit Cards were the most popular payment methods.

- iPhone SE was the top-selling mobile model.

- Most sales occurred during the weekend, with Saturday having the highest.

### Tools Used

- Power BI for Data Visualization and Analysis

### Project Files

- Dataset/ – Contains the dataset file.

- Screenshots/ – Contains images of the dashboard and charts.

- PowerBI_Report.pbix – The Power BI report file.

- README.md – This file explaining the project.

### How to Use This Project

1. Open the provided Power BI (.pbix) file using Power BI Desktop.

2. Explore the interactive visuals using slicers for brand, city, and month filters.

3. Modify the dataset if required and refresh the data model.

4. Export insights using Power BI's export options.

### Requirements

- Power BI Desktop (latest version)

- Microsoft Excel (for reviewing the dataset if needed)

### Contributing
Contributions are welcome. If you have suggestions or want to enhance the dashboard, please feel free to raise an issue or submit a pull request.

### License
This project is open-source under the MIT License. Feel free to modify and use it as needed.

### Credit
Special thanks to [Satish Dhawale](https://www.linkedin.com/in/satish-dhawale/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_recent_activity_content_view%3BhrVX1riLRKCchnte407JRQ%3D%3D). Dataset used from [Skill Course Hindi](https://www.youtube.com/@skillcoursehindi) channel owned by Sathish Dhawale.



