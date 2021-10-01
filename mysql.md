## Browsing
-------------------
- SHOW DATABASES;
- SHOW TABLES;
- SHOW FIELDS FROM table / DESCRIBE table;
- SHOW CREATE TABLE table;
- SHOW PROCESSLIST;
- KILL process_number;

### Select
------------------
- SELECT * FROM table;
- SELECT * FROM table1, table2;
- SELECT field1, field2 FROM table1, table2;
- SELECT ... FROM ... WHERE condition
- SELECT ... FROM ... WHERE condition GROUPBY field;
- SELECT ... FROM ... WHERE condition GROUPBY field HAVING condition2;
- SELECT ... FROM ... WHERE condition ORDER BY field1, field2;
- SELECT ... FROM ... WHERE condition ORDER BY field1, field2 DESC;
- SELECT ... FROM ... WHERE condition LIMIT 10;
- SELECT DISTINCT field1 FROM ...
- SELECT DISTINCT field1, field2 FROM ...

### Select - Join
------------------
- SELECT ... FROM t1 JOIN t2 ON t1.id1 = t2.id2 WHERE condition;
- SELECT ... FROM t1 LEFT JOIN t2 ON t1.id1 = t2.id2 WHERE condition;
- SELECT ... FROM t1 JOIN (t2 JOIN t3 ON ...) ON ...

### Create / Open / Delete Database
------------------
- CREATE DATABASE DatabaseName;
- CREATE DATABASE DatabaseName CHARACTER SET utf8;
- USE DatabaseName;
- DROP DATABASE DatabaseName;
- ALTER DATABASE DatabaseName CHARACTER SET utf8;

### Conditions
------------------
- field1 = value1
- field1 <> value1
- field1 LIKE 'value _ %'
- field1 IS NULL
- field1 IS NOT NULL
- field1 IS IN (value1, value2)
- field1 IS NOT IN (value1, value2)
- condition1 AND condition2
- condition1 OR condition2
