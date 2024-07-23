# My sql

<img src="https://webuilddatabases.com/wp-content/uploads/2015/03/mysql-icon-250x314.png" width="500" height="350">

# Tabel of content

* introduction
* What is mysql
* Installation
* System requirement
* What is Database
* Command types of mysql
* Application of Mysql
* Structure of mysql
* Datatypes
* Primary key & foreign key
* Mysql commands(CRUD)

  ### Introduction
  * MySQL is a relational database management system The database structure is organized into physical files optimized for speed. The logical data model, with objects such as data tables, views, rows, and columns, offers a flexible programming environment.
  
  #### What is Mysql?
  * MySQL is an open-source, Relational Database Management System that stores data in a structured format using rows and columns. It’s software that enables users to create, manage, and manipulate databases. Developed by MySQL AB, which is now owned by Oracle Corporation, MySQL is renowned for its reliability, scalability, and ease of use.
  
 ## Installation 
 * MySQL is one of the most popular relational database management software that is widely used in today's industry. It provides multi-user access support with various storage engines. It is backed by Oracle Company. In this section, we are going to learn how we can download and install MySQL for beginners

 Download MySQL

Follow these steps:
* Step 1: Go to the official website of MySQL and download the community server edition software. Here, you will see the option to choose the Operating System, such as Windows.

* Step 2: Next, there are two options available to download the setup. Choose the version number for the MySQL community server, which you want. If you have good internet connectivity, then choose the mysql-installer-web-community. Otherwise, choose the other one.

<img src="https://static.javatpoint.com/mysql/images/installmysql.png" width="400" height="350">


#### Installing MySQL on Windows

* Step 1: After downloading the setup, unzip it anywhere and double click the MSI installer .exe file. It will give the following screen:
<img src="https://static.javatpoint.com/mysql/images/installmysql2.png" width="400" height="350">

* Step 2: In the next wizard, choose the Setup Type. There are several types available, and you need to choose the appropriate option to install MySQL product and features. Here, we are going to select the Full option and click on the Next button.
<img src="https://static.javatpoint.com/mysql/images/installmysql3.png" width="400" height="350">

* Step 3: Once we click on the Next button, it may give information about some features that may fail to install on your system due to a lack of requirements. We can resolve them by clicking on the Execute button that will install all requirements automatically or can skip them. Now, click on the Next button

<img src="https://static.javatpoint.com/mysql/images/installmysql4.png" width="400" height="350">

* Step 4: In the next wizard, we will see a dialog box that asks for our confirmation of a few products not getting installed. Here,we have to click on the Yes button.

<img src="https://static.javatpoint.com/mysql/images/installmysql5.png" width="400" height="350">

* Step 5: Once we click on the Execute button, it will download and install all the products. After completing the installation, click on the Next button.

<img src="https://static.javatpoint.com/mysql/images/installmysql7.png" width="400" height="350">

* Step 6: In the next wizard, we need to configure the MySQL Server and Router. Here, I am not going to configure the Router because there is no need to use it with MySQL. We are going to show you how to configure the server only. Now, click on the Next button.

<img src="https://static.javatpoint.com/mysql/images/installmysql8.png" width="400" height="350">

* Step 7: Now, the MySQL installation is complete. Click on the Finish button

<img src="https://static.javatpoint.com/mysql/images/installmysql21.png" width="400" height="350">




## Installing Mysql on linux

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

* To run the Linux OS smoothly minimum 1-2 GB RAM is required. The actual minimum memory requirements for the Linux operating system only (without any additional software) are less than these numbers. For example, it is possible to install Debian with 20MB RAM.

* Linux is not too hungry for disk space. To install and use Linux, you should have at least 250 MB of free hard disk space. (The minimum is about 100 MB, but installing Linux on a system with so little disk space will compel you to omit many useful applications and will leave you with little room to work.)

* The address-space limit is system-specific: 32-bit OSes imposes a limit of no more than 4Gb: it is often 3Gb. Running 32-bit executables on a 64-bit OS will have similar limits: 64-bit        executables will have an essentially infinite system-specific limit (e.g., 128Tb for Linux on x86_64 cpus).

* 4 to 5 GB hard disk is enough to store the system and other important files of a Linux distribution. However, to store users' data it is recommended to have at least 25 GB hard disk size.

* Linux requires very little memory to run compared to other advanced operating systems. You should have at the very least 8 MB of RAM; however, it's strongly suggested that you have at least 16    MB. The more memory you have, the faster the system will run.

## What is database?

* A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS)

* A database is an organized collection of data stored in a computer system and usually controlled by a database management system (DBMS). The data in common databases is modeled in tables, making querying and processing efficient. Structured query language (SQL) is commonly used for data querying and writing.

* The Database is an essential part of our life. We encounter several activities that involve our interaction with databases, for example in the bank, in the railway station, in school, in a grocery store, etc. These are the instances where we need to store a large amount of data in one place and fetch these data easily. 

## Command type of mysql?
There are mainly 3 types of SQL commands:

• DDL (Data Definition Language): A Data Definition Language (DDL) refers to a language that is used to modify data and define data structures. For instance, the DDL commands could be used to remove, add, or modify tables within a database

• DML (Data Manipulation Language): A data manipulation language (DML) is a computer programming language used for adding (inserting), deleting, and modifying (updating) data in a database. A DML is often a sublanguage of a broader database language such as Mysql, with the DML comprising some of the operators in the language.

• DCL (Data Control Language):A data control language (DCL) is a syntax similar to a computer programming language used to control access to data stored in a database (authorization). In particular, it is a component of Structured Query Language (SQL). Data Control Language is one of the logical group in SQL Commands.

## Applications of mysql

MySQL is used to store data in tables that map to objects. Each table has a schema defining what columns each row of the table will have. Developers can reliably store and retrieve many data types, including text, numbers, dates, times, and even JSON

*Who uses MySQL? 6458 companies reportedly use MySQL in their tech stacks, including Uber, Airbnb, and Pinterest.

* MySQL is a relational database management system

* Databases are the essential data repository for all software applications. For example, whenever someone conducts a web search, logs in to an account, or completes a transaction, a database system is storing the information so it can be accessed in the future.




