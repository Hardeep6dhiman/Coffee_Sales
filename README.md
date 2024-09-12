# Coffee_Sales

## Project Overview

The Coffee Sales Project is a data analysis and visualization project aimed at analyzing and visualizing sales data from a fictional Coffee restaurant chain. This project utilizes Excel for data extraction, transformation and data visualization. The goal of this project is to provide insights and actionable information to help the Coffee restaurant optimize its operations, improve sales, and enhance customer satisfaction.

## Project Components

### 1. Data Acquisition

The project begins with the acquisition of raw sales data. This data may include information such as customer , product details and order . Data can be obtained from various sources, including databases, CSV files, or other data storage systems.

### 2. Data Gathering with Excel

Microsoft Excel is used to clean, filter, and transform the raw data into a format suitable for analysis. This may involve tasks such as Extracting data, Add columns, Format data types by the use of Excel function such as  as respectively:-

  1. Customer name: Extract customer name from customer table using vlookup.
      Customername:(=VLOOKUP($C2,customers!$A$1:$I$1001,2,0)).
     
  2. Emai: In email column there are many Null values. So extracting data shows error. To resolve this problem I use "IF" function and "VLOOKUP" function.
       Email: (=IF(VLOOKUP($C2,customers!$A$1:$I$1001,3,0)=0,"",VLOOKUP($C2,customers!$A$1:$I$1001,3,0))
     
  3. Country: Extract country from customer table using vlookup.
      Country:(=VLOOKUP($C2,customers!$A$1:$I$1001,7,0)).

  4. Coffee Type,Roast Type, Size, Unit Price: Extract data by using INDEX and MATCH functions.
      Coffee Type: (=INDEX(products!$A$1:$G$49,MATCH(orders!$D3,products!$A$1:$A$49,0),MATCH(orders!$I$1,products!$A$1:$G$1,0))).

  5. Add Column with Coffee Type name, Roast Type name, Loyalty Card: Adding new columns in the table to extract further data. Using "If" statement I extract all the data. Replacing data with new data in these         columns.
      
### 3. Data Analysis

Once the data is prepared, various pivot tables are created for data analysis. This may include:

- Identifying Total Sales over time.
- Analyzing sales trends over time.
- Evaluating Top customers.
- Identifying Sales by country.

### 4. Visualization

Excel is used to create interactive and informative visualizations that showcase the insights gained from the data analysis. The visualizations may include:

- Column charts displaying sales by country.
- Column chart displaying Top Five Customers.
- Line Chart to display Sales and sales trend over time.

### Visualization

![Dashboard ]()


### 5. Insights and Recommendations

Based on the analysis and visualizations, actionable insights and recommendations are provided to the coffee shop. These insights can help in making informed decisions to improve sales, marketing strategies, and overall business performance.

## Dependencies

- Microsoft Excel.
