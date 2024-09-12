# MySQL

<img src="https://webuilddatabases.com/wp-content/uploads/2015/03/mysql-icon-250x314.png" width="500" height="350">

# Table of Content

* [Introduction](#Introduction)
* [What is  MySQL?](#What-is-MySQL?)
* [Installation](#Installation)
* [System requirements](#System-requirements)
* [What is database?](#What-is-database)
* [Datatypes](#Datatypes)
* [Constraints](#Constraints)
* [Application of Mysql CRUD](#Application-of-MySQL-CRUD)
  


 ## Introduction
  * MySQL stands for 'My Structured Query Language' and is a relational database management system. It organizes data into physical files optimized for speed. The logical data model includes objects such as tables, views, rows, and 
    columns, which provide a flexible environment for managing and querying data.
  
 ## What is MySQL?
  * MySQL is an open-source, Relational Database that stores data in a structured format using rows and columns. This software that enables users to create, manage, and manipulate databases. Developed by MySQL AB, 
    which is by Oracle Corporation, MySQL is renowned for its reliability, scalability, and ease of use.
  
 ## Installation 
 * MySQL is one of the most popular relational database software that is widely used in industrys. MySQL provide multi-user access. It is Devloped by Oracle 
   Company. In this Database, we are going to learn how we can download and install MySQL in our system.

 Download MySQL

## Installing MySQL on linux
   Follow these steps:

* Step 1: Open terminal using Ctrl+Alt+T. Now copy and paste the following command in the terminal to install MySQL in Linux.
  ##### sudo apt install mysql-server

```
 harsh@harsh-IdeaPad-3-15IAU7:~$ sudo apt install mysql-server
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  libreoffice-ogltrans libwpe-1.0-1 libwpebackend-fdo-1.0-1
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  mysql-client-8.0 mysql-client-core-8.0 mysql-common mysql-server-8.0
  mysql-server-core-8.0
Suggested packages:
  mailx tinyca
The following NEW packages will be installed:
  mysql-client-8.0 mysql-client-core-8.0 mysql-common mysql-server
  mysql-server-8.0 mysql-server-core-8.0
0 upgraded, 6 newly installed, 0 to remove and 103 not upgraded.
Need to get 7,212 B/21.8 MB of archives.
After this operation, 185 MB of additional disk space will be used.
Do you want to continue? [Y/n]  
Then give your password and hit ENTER.
```

* Step 2: Press “y” to continue.

```
Do you want to continue? [Y/n] y                                              
Get:1 http://in.archive.ubuntu.com/ubuntu jammy/main amd64 mysql-common all 5.8+1.0.8 [7,212 B]
Fetched 7,212 B in 1s (10.8 kB/s)        
Preconfiguring packages ...
Selecting previously unselected package mysql-common.
(Reading database ... 216626 files and directories currently installed.)
Preparing to unpack .../mysql-common_5.8+1.0.8_all.deb ...
Unpacking mysql-common (5.8+1.0.8) ...
Selecting previously unselected package mysql-client-core-8.0.
Preparing to unpack .../mysql-client-core-8.0_8.0.39-0ubuntu0.22.04.1_amd64.deb 
...
Unpacking mysql-client-core-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Selecting previously unselected package mysql-client-8.0.
Preparing to unpack .../mysql-client-8.0_8.0.39-0ubuntu0.22.04.1_amd64.deb ...
Unpacking mysql-client-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Selecting previously unselected package mysql-server-core-8.0.
Preparing to unpack .../mysql-server-core-8.0_8.0.39-0ubuntu0.22.04.1_amd64.deb 
...
Unpacking mysql-server-core-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Setting up mysql-common (5.8+1.0.8) ...
update-alternatives: using /etc/mysql/my.cnf.fallback to provide /etc/mysql/my.c
nf (my.cnf) in auto mode
Selecting previously unselected package mysql-server-8.0.
(Reading database ... 216824 files and directories currently installed.)
Preparing to unpack .../mysql-server-8.0_8.0.39-0ubuntu0.22.04.1_amd64.deb ...
Unpacking mysql-server-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Selecting previously unselected package mysql-server.
Preparing to unpack .../mysql-server_8.0.39-0ubuntu0.22.04.1_all.deb ...
Unpacking mysql-server (8.0.39-0ubuntu0.22.04.1) ...
Setting up mysql-client-core-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Setting up mysql-server-core-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Setting up mysql-client-8.0 (8.0.39-0ubuntu0.22.04.1) ...
Setting up mysql-server-8.0 (8.0.39-0ubuntu0.22.04.1) ...
update-alternatives: using /etc/mysql/mysql.cnf to provide /etc/mysql/my.cnf (my
.cnf) in auto mode
Renaming removed key_buffer and myisam-recover options (if present)
mysqld will log errors to /var/log/mysql/error.log
mysqld is running as pid 10909
Created symlink /etc/systemd/system/multi-user.target.wants/mysql.service → /lib
/systemd/system/mysql.service.
Setting up mysql-server (8.0.39-0ubuntu0.22.04.1) ...
Processing triggers for man-db (2.10.2-1) ...
harsh@harsh-IdeaPad-3-15IAU7:~$ ^C
harsh@harsh-IdeaPad-3-15IAU7:~$
```

##### Verify MySQL Installation

* Step 3: To verify the MySQL installation or to know the version of MySQL. Use this commands in your Terminal.
  ##### mysql --version
```
harsh@harsh-IdeaPad-3-15IAU7:~$ mysql --version
mysql  Ver 8.0.39-0ubuntu0.22.04.1 for Linux on x86_64 ((Ubuntu))
harsh@harsh-IdeaPad-3-15IAU7:~$ 
```

* Step 4: Now we will set the VALIDATE PASSWORD component and starts downloading MySQL in our system.
  ##### sudo mysql_secure_installation
  
```
harsh@harsh-IdeaPad-3-15IAU7:~$  sudo mysql_secure_installation

Securing the MySQL server deployment.

Connecting to MySQL using a blank password.
The 'validate_password' component is installed on the server.
The subsequent steps will run with the existing configuration
of the component.

Skipping password set for root as authentication with auth_socket is used by default.
If you would like to use password authentication instead, this can be done with the "ALTER_USER" command.
See https://dev.mysql.com/doc/refman/8.0/en/alter-user.html#alter-user-password-management for more information.

By default, a MySQL installation has an anonymous user,
allowing anyone to log into MySQL without having to have
a user account created for them. This is intended only for
testing, and to make the installation go a bit smoother.
You should remove them before moving into a production
environment.
```

* Step 5: Then press “n” to set the system password.

```
Remove anonymous users? (Press y|Y for Yes, any other key for No) : n

 ... skipping.


Normally, root should only be allowed to connect from
'localhost'. This ensures that someone cannot guess at
the root password from the network.

Disallow root login remotely? (Press y|Y for Yes, any other key for No) : n

 ... skipping.
By default, MySQL comes with a database named 'test' that
anyone can access. This is also intended only for testing,
and should be removed before moving into a production
environment.


Remove test database and access to it? (Press y|Y for Yes, any other key for No) : n

 ... skipping.
Reloading the privilege tables will ensure that all changes
made so far will take effect immediately.

Reload privilege tables now? (Press y|Y for Yes, any other key for No) : y
Success.

All done! 
harsh@harsh-IdeaPad-3-15IAU7:~$ 

```

* Now the whole setup is done. Hence, MySQL installaion is successfully done!

  MySQL-Successful-Installed-(1)

## System requirements

* To run the Linux OS smoothly minimum 2 GB RAM is required. The actual minimum memory requirements for the Linux operating system only (without any additional software) are less than these numbers. For example, 
  it is possible to install Debian with 1GB RAM.

* Linux does not require much disk space. To install and use Linux, you should have at least 2 GB of free hard disk space.

* The address-space limit is system-specific: 32-bit OSes imposes a limit of no more than 4 GB: it is often 3 GB. Running 32-bit executables on a 64-bit OS will have similar limits: 64-bit executables will have an 
  essentially infinite system-specific limit (e.g., 128Tb for Linux on x86_64 cpus).

* 4 to 5 GB hard disk is enough to store the system and other important files of a Linux distribution. However, to store users' data it is recommended to have at least 25 GB hard disk size.

* Linux requires very little memory to run compared to other advanced operating systems. You should have at the very least 1GB of RAM; however, it's strongly suggested that you have at least 
  1GB. The more memory you have, the faster the system will run.

## What is database?

* A database is an collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS)

* A database is an collection of data stored in a computer system and controlled by a database management system (DBMS). The data in common databases is modeled in tables,making querying and 
  processing efficient. Structured query language (SQL) is commonly used for data querying and writing.

* The Database is an part of our life. We encounter several activities that involve our interaction with databases, for example in the bank, in the railway station, in school, in a grocery store, 
  etc. These are the instances where we need to store a large amount of data in one place and fetch these data easily. 


## Applications of MySQL

MySQL is used to store data in tables that map to objects. Each table has a schema defining what columns each row of the table will have. Developers can reliably store and retrieve many data types, including text, numbers, dates, time
* Who uses MySQL? 6458 companies reportedly use MySQL in their tech stacks, including Uber, Airbnb, and Pinterest.

* MySQL is a relational database management system

* Databases are the essential data repository for all software applications. For example, whenever someone conducts a web search, logs in to an account, or completes a transaction, a database 
  system is storing the information so it can be accessed in the future.
  
## Datatypes
 * Each column in a database table is required to have a name and a data type.

 * An SQL developer must decide what type of data that will be stored inside each column when creating a table. The data type is a guideline for SQL to understand what type of data is expected 
   inside of each column, and it also identifies

### How SQL will interact with the data.
    
 * Data type of a column defines what value the column can store in table
  
 * Defined while creating tables in database
  
 * String: char, varchar, etc
   
 * Numeric: int, float, bool, etc
   

### Commonly used datatype in MySQL

* int: used for the integer value

* float: used to specify a decimal point number

* bool: used to specify Boolean values true and false

* char: fixed length string that can contain numbers, letters, and special characters

* varchar: variable length string that can contain numbers, letters, and special characters

## Constraints:

* Constraints are used to limit the type of data that can go into a table. This ensures the accuracy and reliability of the data in the table. If there is any violation between the constraint 
  and the data action, the action is aborted.

* Constraints are used to specify rules for data in a table

* This ensures the accuracy and reliability of the data in the table

* Constraints can be specified when the table is created with the CREATE TABLE statement

* after the table is created with the ALTER TABLE statement

* Syntax

CREATE TABLE table_name (
column1 datatype constraint,
column2 datatype constraint,
column3 datatype constraint,
....
);


## MySQL application
* CRUD = CRUD is the for CREATE, READ, UPDATE and DELETE. These terms describe the four essential operations for creating and managing persistent data elements, mainly in relational and 
  NoSQL databases

* MySQL provides a set of some basic but most essential operations that will help you to easily interact with the MySQL database and these operations are known as CRUD operations

  <img src="https://www.atatus.com/glossary/content/images/2021/07/CRUD.jpeg" width="400" height="300">
  
* In such apps, users must be able to create data, have access to the data in the UI by reading the data, update or edit the data, and delete the data.

## Use and create database before creating table
* Create database in mysql
  #### CREATE DATABASE harsh;

```
  mysql> CREATE DATABASE harsh;
Query OK, 1 row affected (0.02 sec)


```



#### show databases;

```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| harsh              |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.08 sec)


```
* After that use any of database which is show in at terminal
  #### use harsh
  
```
mysql> use harsh
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed


```
  

### Creating database & tables
  * Datatypes
  * Primary & foregin keys
  * Constraints
  
### Mysql commands
  * create
  * Insert
  * Update
  * Delete
    
  
  ## Creating table
  
The CREATE TABLE statement is used to create a new table in a database
* Syntax

  CREATE TABLE table_name
(
 column_name1 datatype constraint,
 column_name2 datatype constraint,
 column_name3 datatype constraint,
);

* Example

 CREATE TABLE Employee 
 (
 Emp_ID varchar(50) PRIMARY KEY,
 Name char(50),
 Experience int(2),
 Department char(20),
 Salary int(5);
 ```
Query OK, 0 rows affected, 2 warnings (0.02 sec)
mysql> show tables;
+-----------------+
| Tables_in_harsh |
+-----------------+
| Employee        |
+-----------------+
1 row in set (0.00 sec)

```
 

## Insert value in table

  The INSERT INTO statement is used to insert new records in a table
* Syntax

 INSERT INTO TABLE_NAME
 (column1, column2, column3,...columnN)
 VALUES
 (value1, value2, value3,...valueN);

* Example

  INSERT INTO Employee
  (Emp_ID,Name,Experience,Department,Salary)
  VALUES
  ('IT01', ‘Harsh’,5, ‘IT’,75000),
  ('HR02', ‘Aman’, 4, ‘HR’, 60000),
  ('OP03', ‘Hunny’,6, ‘Operation’,90000),
  ('SL04', ‘Abhishek’,6, ‘Sales’,85000);


```
Query OK, 4 rows affected (0.01 sec)
Records: 4  Duplicates: 0  Warnings: 0


mysql> select * from Employee;
+--------+----------+------------+------------+--------+
| Emp_ID | Name     | Experience | Department | Salary |
+--------+----------+------------+------------+--------+
| IT01   | Harsh    |          5 | IT         |  75000 |
| Hr02   | Aman     |          4 | HR         |  60000 |
| OP03   | Hunny    |          6 | Operations |  90000 |
| SL04   | Abhishek |          6 | Sales      |  85000 |
+--------+----------+------------+------------+--------+
4 rows in set (0.00 sec)


```

## Update value in table

  The UPDATE command is used to update existing rows in a table

  * Syntax
  
  UPDATE TABLE_NAME
  SET “Column_name1” = ‘value1’, “Column_name2” = ‘value2’
  WHERE “ID” = ‘value’

* Example

  UPDATE customer
  SET Experience = 10, Salary = 120000
  WHERE Name = 'Harsh';

```
Query OK, 1 row affected (0.01 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> select * from Employee;
+--------+----------+------------+------------+--------+
| Emp_ID | Name     | Experience | Department | Salary |
+--------+----------+------------+------------+--------+
| IT01   | Harsh    |         10 | IT         | 120000 |
| Hr02   | Aman     |          4 | HR         |  60000 |
| OP03   | Hunny    |          6 | Operations |  90000 |
| SL04   | Abhishek |          6 | Sales      |  85000 |
+--------+----------+------------+------------+--------+
4 rows in set (0.00 sec)

```

## Delete values in table

The DELETE statement is used to delete existing records in a table
• Syntax

DELETE FROM table_name WHERE condition;

* Example

DELETE FROM Employee
WHERE Emp_ID = 'Hr02';

```
Query OK, 1 row affected (0.01 sec)

mysql> select * from Employee;
+--------+----------+------------+------------+--------+
| Emp_ID | Name     | Experience | Department | Salary |
+--------+----------+------------+------------+--------+
| IT01   | Harsh    |         10 | IT         | 120000 |
| OP03   | Hunny    |          6 | Operations |  90000 |
| SL04   | Abhishek |          6 | Sales      |  85000 |
+--------+----------+------------+------------+--------+
3 rows in set (0.00 sec)

mysql> 


```
How to exit form terminal after using MySQL?
* Press ctrl+d for exit mysql
```
mysql> ^DBye
harsh@harsh-IdeaPad-3-15IAU7:~$ 


```


## Reference links
* https://www.mysql.com/
* https://www.w3schools.com/MySQL/default.asp
* https://en.wikipedia.org/wiki/MySQL
* https://onecompiler.com/mysql
