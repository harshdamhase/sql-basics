# sql-basics
SQL  

SQL stands for `Structured Query Language` 

SQL lets you access and manipulate databases 

SQL can retrieve data from a database 

SQL can insert records in a database 

SQL can update records in a database 

SQL can delete records from a database 

 ### DIFF BET SQL AND NOSQL

 `SQL` is stored data in tabular format.<br/>
 `NOSQL` is stored data in file format.<br/>

 `SQL` is relational.<br/>
 `NOSQL` is non relational.<br/>

Example of `Nosql` is MongoDB.<br/>
Example of `sql` is MySQL, SQL Server, Oracle<br/>

SQL Supports the ACID properties.<br/>
NoSQL does not support ACID properties.<br/>


The **ORDER BY** keyword is used to sort the result-set in ascending or descending order.


```SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;
```

The AND operator displays a record if all the conditions are TRUE.

The OR operator displays a record if any of the conditions are TRUE.

```
SELECT column1, column2, ...
FROM table_name
WHERE condition1 OR condition2 OR condition3 ...;
```

```
UPDATE table_name 
SET column1 = value1, column2 = value2, ... 
WHERE condition; 
```

The DELETE statement is used to delete existing records in a table.

```DELETE FROM table_name WHERE condition;``` 

 To delete the table completely, use the DROP TABLE statement:
 
 
``CREATE TABLE``` coomand used to create table.

``Syntax:`` 

```CREATE TABLE Tablename(columnname datatype);```

SELECT is used to show all records in table. 

```select * from tablename.```

Table is collection of rows and coloumns. 

The SELECT TOP clause is used to specify the number of records to return.

The `MAX()` function returns the largest value of the selected column. 

The `COUNT()` function returns the number of rows that matches a specified criterion. 

The `AVG()` function returns the average value of a numeric column. 

The `IN` operator allows you to specify multiple values in a WHERE clause.

The **UNION** operator selects only distinct values by default. To allow duplicate values, use UNION ALL: 

```
SELECT column_name(s) FROM table1 
UNION ALL 
SELECT column_name(s) FROM table2;
```

Every SELECT statement within UNION must have the same number of columns 

The columns must also have similar data types 

The columns in every SELECT statement must also be in the same order 

 
```
SELECT column_name(s) FROM table1 
UNION 
SELECT column_name(s) FROM table2;  
```
 
The GROUP BY statement is often used with aggregate functions (COUNT(), MAX(), MIN(), SUM(), AVG()) to group the result-set by one or more columns. 

The HAVING clause was added to SQL because the WHERE keyword cannot be used with aggregate functions.

```
SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
HAVING condition
ORDER BY column_name(s);
```

A stored procedure is a prepared SQL code that you can save, so the code can be reused over and over again. 

```CREATE PROC SP_NAME AS```

To execute stored procedure using 
```EXEC procedure_name``` command.


### VIEW

``VIEW`` Is a virtual represntation of table. WE can create,update and delte view. using commanads.

``CREATE VIEW`` To create a view.
``UPDATE VIEW`` To update view.
``DROP VIEW`` To delete view.

 
### ACID PROPERTY 

``A`` : ATOMICITY 

``C``: CONSISTENCY 

``I``: ISOLATION 

``D``: DURABILITY 

 
``CURSOR``: ROW BY ROW Insertion of records. 

`table` is an independent data object.	
`VIEW` depends on the table. Therefore we cannot create a view without using tables. 

`Table` is a physical entity that means data is actually stored in the table. The `view` is a virtual entity, which means data is not actually stored in the table.

`Page` is used to display the information.

commit and rollback are transactions.

**Rollback** It is used for reverting changes performed by transactions.

`Syntax`

```js
Rollback;
```

**Commit** It is used to storing changes permantly performed by a transaction.

```js
COMMIT;
```

#### ERRORS IN SQL:

1.**Syntax Error**
2.**datatype error**
3. **constraint validation**
4. **semantic error**

### SQL GROUP BY Close

It is used to group rows to have the same values into summary rows


