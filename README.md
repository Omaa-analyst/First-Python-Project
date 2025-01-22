# First-Python-Project

In this project, I worked with a business dataset that provided sales data, including product details, transaction information, and customer insights. The goal was to clean and analyze the data to extract meaningful insights and trends.

1. Importing the Data
The first step involved importing the CSV file that contained the sales data. This file included details like invoice numbers, product codes, quantities sold, unit prices, sales dates, and more.

2. Checking for Missing Data and Filling It
Once the data was loaded, I checked for any missing or null values. Missing data is common in real-world datasets, so I filled these gaps appropriately based on the type of data, using methods like forward filling, backward filling, or setting default values where necessary.

3. Cleaning Data with Regex
I used regular expressions (regex) to clean certain text columns, especially those with inconsistent formats or unnecessary characters. This helped standardize the data, making it easier to analyze and visualize.

4. Handling Date and Time
The dataset included a column called "InvoiceDate," which I converted into a proper datetime format. After conversion, I separated the "InvoiceDate" into two distinct columns: one for the date and one for the time. This allowed me to analyze sales trends by both date and time.

5. Converting Numerical Columns
Columns such as "UnitPrice," "Quantity," and "StockCode" were converted to numeric types to enable mathematical operations and calculations. This step ensured that the data could be used for aggregations and analysis.

6. Stripping the Month Number and Adding Seasons
The dataset had a month number column, which I stripped to extract only the month name (e.g., January, February). Then, I assigned seasons (Winter, Spring, Autumn, Summer) to each month based on the typical calendar divisions, allowing us to analyze sales data by season.

7. Date Modifications and Renaming Columns
I removed the raw date column to reduce redundancy, and changed the month number to the full month name for easier interpretation in visualizations. Additionally, I renamed the columns "Quality" and "Description" to "Sales" and "Product" respectively, to make the names more meaningful in the context of the dataset.

8. Calculating Annual Sales and Country Sales Percentages
I calculated the total sales count for each product in a given year by summing the sales. Then, I calculated the percentage of sales for each country relative to the total sales. This gave insights into the contribution of each country to the overall sales.

9. Analyzing Top Products
Using a count plot, I visualized the top 20 products based on their total sales. This helped identify the most popular products that generated the highest revenue.

10. Most Frequently Purchased Products
I also identified the products that were bought the most frequently, using a count plot. This highlighted products that, while not necessarily high-revenue, had the highest volume of transactions.

11. Sales Trends by Month
To understand seasonal patterns, I used a line plot to display all sales made in each month. I also used a count plot to analyze the frequency of transactions over time, identifying trends like peak buying months.

12. Country-wise Sales
I analyzed sales for each country using both line plots and count plots, which helped visualize the total value of products bought in each country as well as the frequency of purchases. This gave insights into regional sales dynamics.

13. Sales by Season
I looked at how sales performed during different seasons (Winter, Spring, Autumn, Summer). This was visualized through seasonal trends, giving insight into which seasons saw the most sales activity.

14. Outliers Detection and Removal
I visualized outliers in the data using histogram, and then removed those outliers, as they could distort analysis and lead to inaccurate conclusions.

15. Removing Negative and Missing Values
Finally, I cleaned the data further by removing negative values from columns like "UnitPrice" and "Quantity," as negative numbers were unrealistic in a sales context. I also ensured that any remaining NaN (Not a Number) values were handled by removing or filling them, depending on the context.

Conclusion
Through these steps, I transformed the raw sales data into a clean and structured dataset, ready for further analysis and reporting. The visualizations and statistics provided insights into the business's performance, helping to identify trends, customer behaviors, and regional differences in sales.
