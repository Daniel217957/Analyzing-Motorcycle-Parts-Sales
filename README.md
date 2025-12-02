# Analyzing-Motorcycle-Parts-Sales
![Motorcycle](Motorcycle%20folder/d6752a54510f20d69f0ead15d89f25d0.jpg)
## Skills
SQL: Aggregation (SUM), Date Manipulation (EXTRACT), Conditional Logic (CASE WHEN), Grouping (GROUP BY), Sorting and Filtering (WHERE and ORDER BY clauses).
## Project Context
I analyzed this dataset for a company(fictional) that sells motorcycle parts (distributed in 3 warehouses), to gain a better understanding of wholesale revenue by product line, and how this varies month-to-month and across warehouses. 
## What I Analyzed
The image below displays the breakdown of the "sales" dataset by column, data type, and a short description.
<img width="1090" height="596" alt="image" src="https://github.com/user-attachments/assets/b5255c32-8ea1-4701-b902-f53926447a20" />

My task was to calculate the net revenue for each product line and group the results by month and warehouse. The results should be filtered to display only "Wholesale" orders. In addition, the results were to be sorted by product line and month, followed by net revenue in descending order.

## The Query:
<img width="1116" height="261" alt="image" src="https://github.com/user-attachments/assets/de4ce2dc-e07b-4c2f-9c90-2a6af49f8302" />
I selected the `product_line` and `warehouse` columns to categorize the sales data.
I utilized a `CASE` statement to convert the numeric dates into specific month names ('June', 'July', 'August').
I calculated `net_revenue` by subtracting the total payment fees from the sum of the total sales.
I filtered the dataset using `WHERE` to isolate only 'Wholesale' client transactions.
I grouped the data by product line, month, and warehouse to aggregate the revenue figures.
Lastly, I sorted the final results by product line, month, and then by revenue in descending order.

## Result
<img width="1114" height="281" alt="image" src="https://github.com/user-attachments/assets/dbc46916-2968-44d2-8cbb-c4c9c7071a86" />
The result shows that the Engine product line in the Central warehouse in August had the highest revenue for the company, followed closely by the Frame & body product line for the same month and warehouse. View the complete result [here](Motorcycle%20folder/motorcycle%20result.xlsx)
