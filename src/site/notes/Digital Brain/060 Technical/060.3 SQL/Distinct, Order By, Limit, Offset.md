---
{"dg-publish":true,"permalink":"/digital-brain/060-technical/060-3-sql/distinct-order-by-limit-offset/"}
---

1. DISTINCT:
The DISTINCT keyword is used in a SELECT statement to eliminate duplicate values from the result set. It returns only unique values for the specified column(s). Here's an example:

```sql
SELECT DISTINCT column_name
FROM table_name;
```

Example:
Consider a table called "students" with a column named "country." If you want to retrieve a list of unique countries from the table, you can use the DISTINCT keyword:

```sql
SELECT DISTINCT country
FROM students;
```

2. ORDER BY ASC or DESC:
The ORDER BY clause is used to sort the result set in either ascending (ASC) or descending (DESC) order based on one or more columns. ASC sorts the data in ascending order (from lowest to highest), while DESC sorts it in descending order (from highest to lowest). Here's an example:

```sql
SELECT column1, column2
FROM table_name
ORDER BY column1 ASC/DESC;
```

Example:
Assume we have a table named "employees" with columns "name" and "salary." If you want to retrieve the names and salaries of employees sorted in descending order of their salaries, you can use the ORDER BY clause:

```sql
SELECT name, salary
FROM employees
ORDER BY salary DESC;
```

3. LIMIT:
The LIMIT keyword is used to restrict the number of rows returned by a query. It specifies the maximum number of rows to be retrieved from the result set. Here's an example:

```sql
SELECT column1, column2
FROM table_name
LIMIT number_of_rows;
```

Example:
Suppose you have a table called "products" with columns "product_name" and "price." If you want to retrieve the top 5 products with the highest prices, you can use the LIMIT clause:

```sql
SELECT product_name, price
FROM products
ORDER BY price DESC
LIMIT 5;
```

4. OFFSET:
The OFFSET keyword is used in conjunction with the LIMIT keyword to skip a specified number of rows before returning the result set. It allows you to paginate through the result set. Here's an example:

```sql
SELECT column1, column2
FROM table_name
LIMIT number_of_rows
OFFSET offset_value;
```

Example:
Building upon the previous example, if you want to retrieve the next 5 products with the highest prices (skipping the first 5), you can use the OFFSET clause:

```sql
SELECT product_name, price
FROM products
ORDER BY price DESC
LIMIT 5 OFFSET 5;
```

This query will retrieve the 6th to 10th products with the highest prices.

[[Digital Brain/060 Technical/060.3 SQL/060.3 SQL MOC\|060.3 SQL MOC]]