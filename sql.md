# SQL

## Introduction

* SQL is a database computer language designed for the retrieval and management of data in a relational database.

* SQL stands for Structured Query Language.

## A Brief History of SQL

* **1970** - Dr. Edgar F. "Ted" Codd of IBM is known as the father of relational databases, described a relational model for databases.

* **1974** - Structured Query Lamguage appeared.

* **1978** - IBM worked to develop Codd's ideas and released a product named System.

* **1986** - IBM developed the prototype of relational database and standardized by ANSI. The first relational database was released by Relational Software which later came to be known as Oracle.

## SQL Process

When you are executing an SQL command, the SQL engine figures out how to interpret the task.

There are various components included in this process.

These components are :

* **Query Dispatcher**
* **Optimization Engines**
* **Classic Query Engine**
* **SQL Query Engine, etc.**

>Following is a simple diagram showing the SQL Architecture −

![Image](https://www.tutorialspoint.com/sql/images/sql-architecture.jpg)

***

## Categories of SQL

 **1.DDL (Data Definition Language) :**

Data Definition Language consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database.



 **2.DQL (Data Query Language) :**

Data Query Language statements are used for performing queries on the data within schema objects. The purpose of the DQL Command is to get some schema relation based on the query passed to it.


 **3.DML (Data Manipulation Language) :**

The SQL commands that deals with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements.



 **4.DCL (Data Control Language) :**

DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other controls of the database system.


 **5.TCL (Transaction Control Language) :**

 TCL commands deal with the transaction within the database.



## **Various Syntax in SQL**

### SQL SELECT Statement

~~~sql
SELECT column1, column2....columnN
FROM table_name;
~~~


### SQL DROP TABLE Statement

~~~sql
DROP TABLE table_name;
~~~

### SQL TRUNCATE TABLE Statement

~~~Sql
TRUNCATE TABLE table_name;
~~~

### SQL ALTER TABLE Statement

~~~sql
ALTER TABLE table_name {ADD|DROP|MODIFY} column_name {data_ype};
~~~

### SQL ALTER TABLE Statement (Rename)

~~~sql
ALTER TABLE table_name RENAME TO new_table_name;
~~~

### SQL CREATE INDEX Statement

~~~sql
CREATE UNIQUE INDEX index_name
ON table_name ( column1, column2,...columnN);
~~~

### SQL DROP INDEX Statement

~~~sql
ALTER TABLE table_name
DROP INDEX index_name;
~~~

### SQL DESC Statement

~~~sql
DESC table_name;
~~~


### SQL DROP DATABASE Statement

~~~sql
DROP DATABASE database_name;
~~~

### SQL USE Statement

~~~sql
USE database_name;
~~~

### SQL COMMIT Statement

~~~sql
COMMIT;
~~~

### SQL ROLLBACK Statement

~~~sql
ROLLBACK;
~~~

### SQL UPDATE Statement

~~~sql
UPDATE table_name
SET column1 = value1, column2 = value2....columnN=valueN
[ WHERE  CONDITION ];
~~~

### SQL DELETE Statement

~~~sql
DELETE FROM table_name
WHERE  {CONDITION};
~~~

### SQL CREATE DATABASE Statement

~~~sql
CREATE DATABASE database_name;
~~~


***

## **SQL Aggregate Functions**

* SQL aggregation function is used to perform the calculations on multiple rows of a single column of a table. It returns a single value.

### **Types of SQL Aggregation Function**

1. **COUNT FUNCTION**
   * COUNT function is used to count the number of rows in a database table. It can work on both numeric and non-numeric data types.
   * COUNT function uses the COUNT(*) that returns the count of all the rows in a specified table. COUNT(*) considers duplicate and Null.

  

2. **SUM FUNCTION**
   * Sum function is used to calculate the sum of all selected columns. It works on numeric fields only.

   
3. **AVG FUNCTION**
   * The AVG function is used to calculate the average value of the numeric type. AVG function returns the average of all non-Null values.

  
4. **MAX FUNCTION**
   * MAX function is used to find the maximum value of a certain column. This function determines the largest value of all selected values of a column.

    
5. **MIN FUNCTION**
   * MIN function is used to find the minimum value of a certain column. This function determines the smallest value of all selected values of a column.
***
## **SQL Join (Inner, Left, Right and Full Joins)**

A SQL Join statement is used to combine data or rows from two or more tables based on a common field between them. Different types of Joins are:

* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* FULL JOIN


### INNER JOIN

***

The INNER JOIN keyword selects all rows from both the tables as long as the condition satisfies. This keyword will create the result-set by combining all rows from both the tables where the condition satisfies i.e value of the common field will be the same.

> Syntax:

~~~sql
SELECT tableA.column1,tableA.column2,tableB.column1,....
FROM tableA 
INNER JOIN tableB
ON tableA.matching_column = tableB.matching_column;
~~~



### LEFT JOIN

***

This join returns all the rows of the table on the left side of the join and matching rows for the table on the right side of the join. For the rows for which there is no matching row on the right side, the result-set will contain null. LEFT JOIN is also known as LEFT OUTER JOIN.

> Syntax:

~~~sql
SELECT tableA.column1,tableA.column2,tableB.column1,....
FROM tableA
LEFT JOIN tableB
ON tableA.matching_column = tableB.matching_column;
~~~



### RIGHT JOIN

***

RIGHT JOIN is similar to LEFT JOIN. This join returns all the rows of the table on the right side of the join and matching rows for the table on the left side of the join. For the rows for which there is no matching row on the left side, the result-set will contain null. RIGHT JOIN is also known as RIGHT OUTER JOIN.

> Syntax:

~~~sql
SELECT tableA.column1,tableA.column2,tableB.column1,....
FROM tableA
RIGHT JOIN tableB
ON tableA.matching_column = tableB.matching_column;
~~~



### FULL JOIN

***

FULL JOIN creates the result-set by combining the result of both LEFT JOIN and RIGHT JOIN. The result-set will contain all the rows from both tables. For the rows for which there is no matching, the result-set will contain NULL values.

> Syntax:

~~~sql
SELECT tableA.column1,tableA.column2,tableB.column1,....
FROM tableA
FULL JOIN tableB
ON tableA.matching_column = tableB.matching_column;
~~~




## Conclusion

Thus a large amount of data can be stored and manipulated according to the user requirement. All the above data gives us the foundational tools of understanding how to build and manipulate databases. 
