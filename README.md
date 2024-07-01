# Vrinda-store-annual-Report


## Problem Statement

This dashboard helps the vrinda store to understand their 2022 sales better so that they can grow their sales in 2023. It helps them to know if their customers are satisfied with their services through different visualizations, they get to know their improvement area, & thus they can improve their services by identifying these area.

### Steps followed 

- Step 1 : Load data into Excel, dataset is a csv file.
- Step 2 : Open power query editor to clean the data & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : Check the datatype of all the columns,it is observed that quantity column is in text datatype so change it into number datatype before that replace the text "one" into Number "1". 
- Step 6 : Data processing is done using various functions. 
- Step 7 : Add column "Age Group" and to calculate "Age group" from "Age" column Use "NestedIF" logical function.

            Age group = IF(E2>=50,"Senior",IF(E2>=30,"Adult","Teenager"))

- Step 8 : Add column "Month" and to find month from "date" column use "Text" logical function.

             Month = TEXT(G2,"mmmm")
 
- Step 9 : Go to insert and insert pivot table in new sheet and then choose fields to add to report, add "Month" field in row and "Amount"(sum of sales) and "Order ID"(Count of orders) fields in values. 
![Screenshot 2024-07-01 134414](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/fdcfb4bf-5ba9-4785-b5bf-3029e63efb92)

Pivot table

![Screenshot 2024-07-01 134604](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/20a495a9-395b-4612-aa89-522bfb7fc779)
- Step 10 : Go to pivot table analyze and insert combo pivot chart and then change the chart type "Amount" into Column and "Order ID" into line and add secondory axis for proper visualization. 
![Screenshot 2024-07-01 142635](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/fc34be22-9328-4957-bb27-508911d5d752)
- Step 11 : To show men vs women sales, go to insert and insert pivot table in new sheet and then choose fields to add to report, add "Gender" field in row and "Amount"(sum of sales) field in values and then go to pivot table analyze and insert pie pivot chart.
![Screenshot 2024-07-01 142651](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/7cd6c3ff-b348-46cd-a8bc-643f921b8ac2)
- Step 12 : To show order status, go to insert and insert pivot table in new sheet and then choose fields to add to report, add "Status" field in row and "Order ID"(count of order) field in values and then go to pivot table analyze and insert pie pivot chart.
![Screenshot 2024-07-01 144131](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/4002c689-13bb-4364-baef-ab3a19ae6128)

- Step 13 : To show relation between age and gender based on no of orders, go to insert and insert pivot table in new sheet and then choose fields to add to report, add "Age group" field in row, "Gender" field in column and "Order ID"(percentage of orders) field in values and then go to pivot table analyze and insert clustered bar pivot chart.
![Screenshot 2024-07-01 151120](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/e0cbcd0d-5a8b-4511-8bcd-2591ec0fd2de)

- Step 14 : To show top 10 states according to sales, go to insert and insert pivot table in new sheet and then choose fields to add to report, add "states" field in row and "Amount"(sum of sales) field in values and then go to pivot table analyze and insert bar pivot chart.
![Screenshot 2024-07-01 151106](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/1f76eb5a-bc69-4229-ba62-975094f697e5)

- Step 15 : To show channel wise orders, go to insert and insert pivot table in new sheet and then choose fields to add to report, add "Channel" field in row and "Order ID"(count of order) field in values and then go to pivot table analyze and insert pie pivot chart.
![Screenshot 2024-07-01 170012](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/59c2526e-8dc5-47c6-b403-bf80b2bc9879)
- Step 16 : Visual filters (Slicers) were added for two fields named "Month" and "Category". 

 
 - Step 17 : The report was then published.

 
 # Report Snapshot (Power BI DESKTOP)

 
![Screenshot 2024-07-01 170715](https://github.com/Smitamane25/Ecommerce-Sales-Dashboard/assets/171058471/5bfbe2d7-62c2-4e91-8640-0ac3ae76665b)

# Insights

1. Women are more likely to buy compared to men(65%).

2. Maharashtra,Karnataka and Uttar Pradesh are top 3 states in sales contribution.

3. Adult age group (30-49) is max contributing.

4. Amazon, Flipkart and Myntra channels are max contributing.
