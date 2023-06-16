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
| Operator |	Condition	| Example |
| ____
=	Case sensitive exact string comparison (notice the single equals)	col_name = "abc"
!= or <>	Case sensitive exact string inequality comparison	col_name != "abcd"
LIKE	Case insensitive exact string comparison	col_name LIKE "ABC"
NOT LIKE	Case insensitive exact string inequality comparison	col_name NOT LIKE "ABCD"
%	Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE)	col_name LIKE "%AT%"
(matches "AT", "ATTIC", "CAT" or even "BATS")
_	Used anywhere in a string to match a single character (only with LIKE or NOT LIKE)	col_name LIKE "AN_"
(matches "AND", but not "AN")
IN (…)	String exists in a list	col_name IN ("A", "B", "C")
NOT IN (…)	String does not exist in a list	col_name NOT IN ("D", "E", "F")  ___ |

