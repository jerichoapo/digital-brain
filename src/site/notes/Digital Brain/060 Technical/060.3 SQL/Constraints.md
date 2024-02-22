---
{"dg-publish":true,"permalink":"/digital-brain/060-technical/060-3-sql/constraints/"}
---

| Operator                | Condition                                 | Example                       |
|-------------------------|-------------------------------------------|-------------------------------|
| =, !=, <, <=, >, >=     | Standard numerical operators              | col_name != 4                |
| BETWEEN ... AND ...     | Number is within range of two values       | col_name BETWEEN 1.5 AND 10.5 |
| NOT BETWEEN ... AND ... | Number is not within range of two values   | col_name NOT BETWEEN 1 AND 10 |
| IN (...)                | Number exists in a list                   | col_name IN (2, 4, 6)         |
| NOT IN (...)            | Number does not exist in a list            | col_name NOT IN (1, 3, 5)     |
| =                       | Case sensitive exact string comparison              | col_name = "abc"              |
| != or <>                | Case sensitive exact string inequality comparison   | col_name != "abcd"            |
| LIKE                    | Case insensitive exact string comparison            | col_name LIKE "ABC"            |
| NOT LIKE                | Case insensitive exact string inequality comparison | col_name NOT LIKE "ABCD"       |
| %                       | Used anywhere in a string to match a sequence       | col_name LIKE "%AT%"           |
|                         | of zero or more characters (only with LIKE or NOT   | (matches "AT", "ATTIC",       |
|                         | LIKE)                                               | "CAT" or even "BATS")         |
| _                       | Used anywhere in a string to match a single         | col_name LIKE "AN_"            |
|                         | character (only with LIKE or NOT LIKE)              | (matches "AND", but not "AN") |
| IN (...)                | String exists in a list                             | col_name IN ("A", "B", "C")    |
| NOT IN                  | String does not exist in a list                     | col_name NOT IN ("D", "E", "F")|
[[Digital Brain/060 Technical/060.3 SQL/060.3 SQL MOC\|060.3 SQL MOC]]