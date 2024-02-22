---
{"dg-publish":true,"permalink":"/digital-brain/060-technical/060-3-sql/basics/"}
---

Think of a table in SQL as a type of an entity (ie. Dogs), and each row in that table as a specific _instance_ of that type (ie. A pug, a beagle, a different colored pug, etc). This means that the columns would then represent the common properties shared by all instances of that entity (ie. Color of fur, length of tail, etc).

1. SELECT:
   - Definition: Used to retrieve data from one or more database tables.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table_name;
     ```
   - Explanation: Retrieves the specified columns (`column1` and `column2`) from the table (`table_name`).

2. FROM:
   - Definition: Specifies the table from which data is being retrieved.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table_name;
     ```
   - Explanation: Specifies the source table (`table_name`) from which the data is being selected.

3. WHERE:
   - Definition: Filters data based on specified conditions.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table_name WHERE condition;
     ```
   - Explanation: Retrieves data from the table (`table_name`) where the specified condition is met.

4. GROUP BY:
   - Definition: Groups rows based on specified columns.
   - Code Example: 
     ```
     SELECT column1, COUNT(column2) FROM table_name GROUP BY column1;
     ```
   - Explanation: Groups the rows by the specified column (`column1`) and applies an aggregate function (`COUNT`) to another column (`column2`).

5. HAVING:
   - Definition: Filters groups based on specified conditions.
   - Code Example: 
     ```
     SELECT column1, COUNT(column2) FROM table_name GROUP BY column1 HAVING condition;
     ```
   - Explanation: Filters the groups created by `GROUP BY` based on the specified condition.

6. ORDER BY:
   - Definition: Sorts the result set based on specified columns.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table_name ORDER BY column1 ASC;
     ```
   - Explanation: Sorts the result set in ascending (`ASC`) or descending (`DESC`) order based on the specified column (`column1`).

7. JOIN:
   - Definition: Combines rows from multiple tables based on a related column between them.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table1 JOIN table2 ON table1.column = table2.column;
     ```
   - Explanation: Combines rows from `table1` and `table2` based on the related column (`column`).

8. INNER JOIN:
   - Definition: Returns only the matching rows between multiple tables.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table1 INNER JOIN table2 ON table1.column = table2.column;
     ```
   - Explanation: Returns only the rows where there is a match between `table1` and `table2` based on the related column (`column`).

9. LEFT JOIN:
   - Definition: Returns all rows from the left table and matching rows from the right table.
   - Code Example: 
     ```
     SELECT column1, column2 FROM table1 LEFT JOIN table2 ON table1.column = table2.column;
     ```
   - Explanation: Returns all rows from `table1` and the matching rows from `table2` based on the related column (`column`).

10. UNION:
    - Definition: Combines the result sets of two or more SELECT statements into a single result set.
    - Code Example: 
      ```
      SELECT column1, column2 FROM table1 UNION SELECT column1, column2 FROM table2;
      ```
    - Explanation: Combines the results of the first SELECT statement with the results of the second SELECT statement, removing any duplicates.

[[Digital Brain/060 Technical/060.3 SQL/060.3 SQL MOC\|060.3 SQL MOC]]