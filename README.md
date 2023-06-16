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

 1.=, !=, < <=, >, >=   col_name != 4<br>
 2.BETWEEN … AND …      col_name BETWEEN 1.5 AND 10.5<br>
 3.NOT BETWEEN … AND    col_name NOT BETWEEN 1 AND 10<br>
 4.IN (…)	              col_name IN (2, 4, 6)<br>
 5.NOT IN (…)           col_name NOT IN (1, 3, 5)<br>

