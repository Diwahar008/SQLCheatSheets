# cheetsheat for  SQL 

**creating new databases**

```sql
create databases new();
```
**to select or use database**
```sql
use database_name;
```
**to select table**
```sql
selct * from table_name;
```
**to select column in table**
```sql
select column_name from table_name;
```

**describe datatype of table**
```sql
describe table_name;
```
**to insert data**
```sql
insert into table_name() values();
```
**to delete table**
```sql
delete table table_name;
```
**Queries with constraints**
```sql
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```   
 | Operator                |    SQL Example                 |
 | ----------------------- |  ----------------------------- |
 | 1.`=, !=, < <=, >, >=`  | col_name != 4 |
 | 2.`BETWEEN … AND … `    | col_name BETWEEN 1.5 AND 10.5 |
 | 3.`NOT BETWEEN … AND`   | col_name NOT BETWEEN 1 AND 10 | 
 | 4.`IN (…)`	           | col_name IN (2, 4, 6) |
 | 5.`NOT IN (…)`          | col_name NOT IN (1, 3, 5) |
 | 6.`=`                   | col_name = "abc" |
 | 7.`!= or <>`            | col_name != "abcd" |
 | 8.`LIKE`                | col_name LIKE "ABC" | 
 | 9.`NOT LIKE`	           | col_name NOT LIKE "ABCD" |
 | 10.`%`                  | col_name LIKE "%AT%" (matches "AT", "ATTIC", "CAT" or even "BATS") |
 | 11.`_`                  | col_name LIKE "AN_" (matches "AND", but not "AN") |
 | 12. `IN (…)`            | col_name IN ("D", "E", "F") |
 | 13. `NOT IN (…)`        | col_name NOT IN ("D", "E", "F") |

Since the DISTINCT keyword will blindly remove duplicate rows, we will learn in a future lesson how to discard duplicates based on specific columns using grouping and the GROUP BY clause.

```
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```

**Filtering and sorting Query results**

```
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
```

**Multi-table queries with JOINs**

```
SELECT column, another_table_column, …
FROM mytable
INNER JOIN another_table 
    ON mytable.id = another_table.id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;
```


