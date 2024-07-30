# My sql

<img src="https://webuilddatabases.com/wp-content/uploads/2015/03/mysql-icon-250x314.png" width="500" height="350">

# Tabel of content

* introduction
* What is mysql
* Installation
* System requirement
* What is Database
* Command types of mysql
* Datatypes
* Primary key & foreign key
* Constraints
* Application of Mysql CRUD
* Joins in mysql


 ## Introduction
  * MySQL is a relational database management system The database structure is organized into physical files optimized for speed. The logical data model, with objects such as data tables, 
    views,       rows, and columns, offers a flexible programming environment.
  
 ## What is Mysql?
  * MySQL is an open-source, Relational Database Management System that stores data in a structured format using rows and columns. It’s software that enables users to create, manage, and           manipulate databases. Developed by MySQL AB, which is now owned by Oracle Corporation, MySQL is renowned for its reliability, scalability, and ease of use.
  
 ## Installation 
 * MySQL is one of the most popular relational database management software that is widely used in today's industry. It provides multi-user access support with various storage engines. It is      backed by Oracle Company. In this section, we are going to learn how we can download and install MySQL for beginners

 Download MySQL

## Installing Mysql on linux
Follow these steps:

* Step 1: Open terminal using Ctrl+Alt+T. Now copy and paste the following command in the terminal to install MySQL in Linux.
  ##### sudo apt install mysql-server

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212153900/Install-MySQL-on-Linux_1.png" width="400" height="300">

Then give your password and hit ENTER. 

* Step 2: Press “y” to continue.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212154030/Install-MySQL-on-Linux_2-(1).jpg" width="400" height="300">

* It will take some time to download and install MySQL in Linux.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212154135/Install-MySQL-on-Linux_3.jpg" width="400" height="300">

##### Verify MySQL Installation

* Step 3: To verify the MySQL installation or to know the version enter the following commands in your Terminal.
  ##### mysql --version

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212154344/Verify-MySQL-Installation_1-(1).jpg" width="400" height="300">

* Step 4: Now we will set the VALIDATE PASSWORD component.
  ##### sudo mysql_secure_installation

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212154459/Protecting-and-Securing-MySQL_1-(1).jpg" width="400" height="300">

* Step 5: Then press “y” to set the password. Next press “0” for the low-level password or choose as you want to set the password.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212154650/Protecting-and-Securing-MySQL_2-(1).jpg" width="400" height="300">

* Step 6: Create a password. Then Re-enter the password, then to continue press “y”.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212154827/Protecting-and-Securing-MySQL_3-(1).jpg" width="400" height="300">

* Now the whole setup is done. Hence, MySQL installaion is successfully done!

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231212155108/MySQL-Successful-Installed-(1).jpg" width="400" height="300">

MySQL-Successful-Installed-(1)

## System requirement

* To run the Linux OS smoothly minimum 1-2 GB RAM is required. The actual minimum memory requirements for the Linux operating system only (without any additional software) are less than these        numbers. For example, it is possible to install Debian with 20MB RAM.

* Linux is not too hungry for disk space. To install and use Linux, you should have at least 250 MB of free hard disk space. (The minimum is about 100 MB, but installing Linux on a system with so    little disk space will compel you to omit many useful applications and will leave you with little room to work.)

* The address-space limit is system-specific: 32-bit OSes imposes a limit of no more than 4Gb: it is often 3Gb. Running 32-bit executables on a 64-bit OS will have similar limits: 64-bit             executables will have an essentially infinite system-specific limit (e.g., 128Tb for Linux on x86_64 cpus).

* 4 to 5 GB hard disk is enough to store the system and other important files of a Linux distribution. However, to store users' data it is recommended to have at least 25 GB hard disk size.

* Linux requires very little memory to run compared to other advanced operating systems. You should have at the very least 8MB of RAM; however, it's strongly suggested that you have at least 
  16MB. The more memory you have, the faster the system will run.

## What is database?

* A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system     (DBMS)

* A database is an organized collection of data stored in a computer system and usually controlled by a database management system (DBMS). The data in common databases is modeled in tables,          making  querying and processing efficient. Structured query language (SQL) is commonly used for data querying and writing.

* The Database is an essential part of our life. We encounter several activities that involve our interaction with databases, for example in the bank, in the railway station, in school, in a         grocery store, etc. These are the instances where we need to store a large amount of data in one place and fetch these data easily. 

## Command type of mysql?
There are mainly 3 types of SQL commands:

• DDL (Data Definition Language): A Data Definition Language (DDL) refers to a language that is used to modify data and define data structures. For instance, the DDL commands could be used to        remove, add, or modify tables within a database

• DML (Data Manipulation Language): A data manipulation language (DML) is a computer programming language used for adding (inserting), deleting, and modifying (updating) data in a database. A 
      DML    is often a sublanguage of a broader database language such as Mysql, with the DML comprising some of the operators in the language.

• DCL (Data Control Language):A data control language (DCL) is a syntax similar to a computer programming language used to control access to data stored in a database (authorization). In             particular, it is a component of Structured Query Language (SQL). Data Control Language is one of the logical group in SQL Commands.

## Applications of mysql

 MySQL is used to store data in tables that map to objects. Each table has a schema defining what columns each row of the table will have. Developers can reliably store and retrieve many data   types, including text, numbers, dates, times, and even JSON

* Who uses MySQL? 6458 companies reportedly use MySQL in their tech stacks, including Uber, Airbnb, and Pinterest.

* MySQL is a relational database management system

* Databases are the essential data repository for all software applications. For example, whenever someone conducts a web search, logs in to an account, or completes a transaction, a database 
  system is storing the information so it can be accessed in the future.
## Datatypes
 * Each column in a database table is required to have a name and a data type.

 * An SQL developer must decide what type of data that will be stored inside each column when creating a table. The data type is a guideline for SQL to understand what type of data is expected 
   inside of each column, and it also identifies

### How SQL will interact with the stored data.
    
 * Data type of a column defines what value the column can store in table
  
 * Defined while creating tables in database
  
 * Data types mainly classified into three categories +most used
  
 * String: char, varchar, etc
   
 * Numeric: int, float, bool, etc
   
 * Date and time: date, datetime, etc

### Commonly used datatype in mysql

* int: used for the integer value

* float: used to specify a decimal point number

* bool: used to specify Boolean values true and false

* char: fixed length string that can contain numbers, letters, and special characters

* varchar: variable length string that can contain numbers, letters, and special characters

* date: date format YYYY-MM-DD

* datetime: date & time combination, format is YYYY-MM-DD hh:mm:ss

## Primary key

* The PRIMARY KEY constraint uniquely identifies each record in a table.

* Primary keys must contain UNIQUE values, and cannot contain NULL values.

* A table can have only ONE primary key; and in the table, this primary key can consist of single or multiple columns (fields).

* A Primary key is a unique column we set in a table to easily identify and locate data in queries

* A table can have only one primary key, which should be unique and NOT NULL
  
## Foreign key

* The FOREIGN KEY constraint is used to prevent actions that would destroy links between tables.

* A FOREIGN KEY is a field (or collection of fields) in one table, that refers to the PRIMARY KEY in another table.

* The table with the foreign key is called the child table, and the table with the primary key is called the referenced or parent table.

* A Foreign key is a column used to link two or more tables together
  
* A table can have any number of foreign keys, can contain duplicateand NULL values
  

## Constraints:

* Constraints are used to limit the type of data that can go into a table. This ensures the accuracy and reliability of the data in the table. If there is any violation between the constraint 
  and the data action, the action is aborted.

* Constraints are used to specify rules for data in a table

* This ensures the accuracy and reliability of the data in the table

* Constraints can be specified when the table is created with the CREATE TABLE statement, or

* after the table is created with the ALTER TABLE statement

* Syntax

CREATE TABLE table_name (
column1 datatype constraint,
column2 datatype constraint,
column3 datatype constraint,
....
);

### Commanly used constraints

* NOT NULL - Ensures that a column cannot have a NULL value

* UNIQUE - Ensures that all values in a column are different

* PRIMARY KEY - A combination of a NOT NULL and UNIQUE

* FOREIGN KEY - Prevents actions that would destroy links between tables (used to link multiple tables together)

* CHECK - Ensures that the values in a column satisfies a specific condition

* DEFAULT - Sets a default value for a column if no value is specified

* CREATE INDEX - Used to create and retrieve data from the database very quickly

## Mysql application
* CRUD =CRUD is the acronym for CREATE, READ, UPDATE and DELETE. These terms describe the four essential operations for creating and managing persistent data elements, mainly in relational and 
  NoSQL databases

* MySQL provides a set of some basic but most essential operations that will help you to easily interact with the MySQL database and these operations are known as CRUD operations

  <img src="https://www.atatus.com/glossary/content/images/2021/07/CRUD.jpeg" width="400" height="300">
  
* In such apps, users must be able to create data, have access to the data in the UI by reading the data, update or edit the data, and delete the data.


### Creating database & tables
  * Datatypes
  * Primary & foregin keys
  * Constraints
  
### Mysql commands
  * create
  * Insert
  * Update
  * Delete
    
  
  ## Creating tabel
  
The CREATE TABLE statement is used to create a new table in a database
* Syntax

  CREATE TABLE table_name
(
 column_name1 datatype constraint,
 column_name2 datatype constraint,
 column_name3 datatype constraint,
);

* Example

 CREATE TABLE customer
(
 CustID int8 PRIMARY KEY,
 CustName varchar(50) NOT NULL,
 Age int NOT NULL,
 City char(50),
 Salary numeric
);

## Insert value in table

  The INSERT INTO statement is used to insert new records in a table
* Syntax

 INSERT INTO TABLE_NAME
 (column1, column2, column3,...columnN)
 VALUES
 (value1, value2, value3,...valueN);

* Example

  INSERT INTO customer
  (CustID, CustName, Age, City, Salary)
  VALUES
  (1, ‘Sam’, 26, ‘Delhi’, 9000),
  (2, ‘Ram’, 19, ‘Bangalore’, 11000),
  (3, ‘Pam’, 31, ‘Mumbai’, 6000),
  (4, ‘Jam’, 42, ‘Pune’, 10000);

## Update value in table

  The UPDATE command is used to update existing rows in a table

  * Syntax
  
  UPDATE TABLE_NAME
  SET “Column_name1” = ‘value1’, “Column_name2” = ‘value2’
  WHERE “ID” = ‘value’

* Example

  UPDATE customer
  SET CustName = 'Xam’, Age= 32
  WHERE CustID = 4;

## Deleter values in table

The DELETE statement is used to delete existing records in a table
• Syntax

DELETE FROM table_name WHERE condition;

* Example

DELETE FROM customer
WHERE CustID = 3;

## Joins in my sql

* JOIN means to combine something.
* A JOIN clause is used to combine data from two ormore tables, based on a related column between them
* A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

### Supported Types of Joins in MySQL

* INNER JOIN: Returns records that have matching values in both tables
* LEFT JOIN: Returns all records from the left table, and the matched records from the right table
* RIGHT JOIN: Returns all records from the right table, and the matched records from the left table
* Full outer  JOIN: Returns all records from both tables
     
### Inner join
* Syntax

  SELECT column_name(s)
  FROM TableA
  INNER JOIN TableB
  ON TableA.col_name = TableB.col_name

* Example

* SELECT 
  FROM customer AS c
  INNER JOIN payment AS p
  ON c.customer_id = p.customer_id

### Left join

* Returns all records from the left table, and the matched records from the right table
  
* Syntax

  SELECT column_name(s)
  FROM TableA
  LEFT JOIN TableB
  ON TableA.col_name = TableB.col_name

* Example

  SELECT *
  FROM customer AS c
  LEFT JOIN payment AS p
  ON c.customer_id = p.customer_id

  ### Right join
  
* Returns all records from the right table, and the matched records from the left table

* Syntax

  SELECT column_name(s)
  FROM TableA
  RIGHT JOIN TableB
  ON TableA.col_name = TableB.col_name

* Example

  SELECT *
  FROM customer AS c
  RIGHT JOIN payment AS p
  ON c.customer_id = p.customer_id

  ### Full join
* Returns all records when there is a match in either left or right table
 
* Syntax

 SELECT column_name(s)
 FROM TableA
 FULL OUTER JOIN TableB
 ON TableA.col_name = TableB.col_name

* Example

 SELECT *
 FROM customer AS c
 FULL OUTER JOIN payment AS p
 ON c.customer_id = p.customer_id

### Which joins to use 

* INNER JOIN: Returns records that have matching values in both tables

* LEFT JOIN: Returns all records from the left table, and the matched records from the right table

* RIGHT JOIN: Returns all records from the right table, and the matched records from the left table

* FULL JOIN: Returns all records when there is a match in either left or right table








