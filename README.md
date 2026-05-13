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
    COUNT(order_id) as total_orders
FROM
    order_details;
```
## question 4
Find the total number of pizzas sold.
```sql
select
 sum(quantity) as total_pizza_sold
from
order_details;
```
## question 5
List all pizza sizes available.
```sql
SELECT DISTINCT
    size
FROM
    pizzas;
```
## question 6
Show the distinct pizza categories.
```sql
SELECT DISTINCT
    category AS pizza_category
FROM
    pizza_types
    order by pizza_category asc;
```
## question 7
Find the earliest order date.
```sql
SELECT 
    MIN(date)
FROM
    orders;
```
## question 8
Find the latest order date.
```sql
SELECT 
    MAX(date)
FROM
    orders;
```
## question 9
Display all pizzas with their prices.
```sql
SELECT 
    pt.name, p.price
FROM
    pizza_types AS pt
        JOIN
    pizzas AS p
 ON pt.pizza_type_id = p.pizza_type_id;
```














