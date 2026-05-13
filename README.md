 # Pizza Sales SQL Analysis Project
This is a SQL data analysis project based on a pizza sales dataset. 
The goal of this project is to practice SQL queries, improve business understanding, 
and analyze sales performance using real-world data.

## Question 1
Show all records from the orders table.

```sql
SELECT * 
FROM orders;
```
## Question 2
Show all pizza names available in the dataset.
```sql
SELECT 
    name
FROM
    pizza_types;
```
## Question 3
Find the total number of orders placed.
```sql
SELECT 
    COUNT(order_details_id)
FROM
    order_details;
```
