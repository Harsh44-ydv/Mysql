# My sql

<img src="https://webuilddatabases.com/wp-content/uploads/2015/03/mysql-icon-250x314.png" width="500" height="350">

# Tabel of content

* introduction
* What is mysql
* Installation
* System requirement
* What is Database
* Applications
* Structure of mysql
* Datatypes
* Primary key & foreign key
* Mysql commands(CRUD)

  ### Introduction
  MySQL is a relational database management system The database structure is organized into physical files optimized for speed. The logical data model, with objects such as data tables, views, rows, and columns, offers a flexible programming environment.
  
  #### What is Mysql?
  MySQL is an open-source, Relational Database Management System that stores data in a structured format using rows and columns. It’s software that enables users to create, manage, and manipulate databases. Developed by MySQL AB, which is now owned by Oracle Corporation, MySQL is renowned for its reliability, scalability, and ease of use.
  
 ## Installation 
 MySQL is one of the most popular relational database management software that is widely used in today's industry. It provides multi-user access support with various storage engines. It is backed by Oracle Company. In this section, we are going to learn how we can download and install MySQL for beginners

 Download MySQL

Follow these steps:
Step 1: Go to the official website of MySQL and download the community server edition software. Here, you will see the option to choose the Operating System, such as Windows.

Step 2: Next, there are two options available to download the setup. Choose the version number for the MySQL community server, which you want. If you have good internet connectivity, then choose the mysql-installer-web-community. Otherwise, choose the other one.
how to install mysql

#### Installing MySQL on Windows

Step 1: After downloading the setup, unzip it anywhere and double click the MSI installer .exe file. It will give the following screen:


Step 2: In the next wizard, choose the Setup Type. There are several types available, and you need to choose the appropriate option to install MySQL product and features. Here, we are going to select the Full option and click on the Next button.

Step 3: Once we click on the Next button, it may give information about some features that may fail to install on your system due to a lack of requirements. We can resolve them by clicking on the Execute button that will install all requirements automatically or can skip them. Now, click on the Next button

Step 4: In the next wizard, we will see a dialog box that asks for our confirmation of a few products not getting installed. Here, we have to click on the Yes button.

Step 5: Once we click on the Execute button, it will download and install all the products. After completing the installation, click on the Next button.

#### Installing Mysql on linux

Step 1: Open terminal using Ctrl+Alt+T. Now copy and paste the following command in the terminal to install MySQL in Linux.
##### sudo apt install mysql-server
Then give your password and hit ENTER. 

Step 2: Press “y” to continue.
It will take some time to download and install MySQL in Linux.

Install-MySQL-on-Linux_3

##### Verify MySQL Installation

Step 3: To verify the MySQL installation or to know the version enter the following commands in your Terminal.

##### mysql --version

Protecting and Securing MySQL

Step 4: Now we will set the VALIDATE PASSWORD component.

### sudo mysql_secure_installation

Step 5: Then press “y” to set the password. Next press “0” for the low-level password or choose as you want to set the password.

Protecting-and-Securing-MySQL_2

Step 6: Create a password. Then Re-enter the password, then to continue press “y”.

Protecting-and-Securing-MySQL_3-(1)

Now the whole setup is done. Hence, MySQL installaion is successfully done!

MySQL-Successful-Installed-(1)

## System requirement

To run the Linux OS smoothly minimum 1-2 GB RAM is required. The actual minimum memory requirements for the Linux operating system only (without any additional software) are less than these numbers. For example, it is possible to install Debian with 20MB RAM.

Linux is not too hungry for disk space. To install and use Linux, you should have at least 250 MB of free hard disk space. (The minimum is about 100 MB, but installing Linux on a system with so little disk space will compel you to omit many useful applications and will leave you with little room to work.)

The address-space limit is system-specific: 32-bit OSes imposes a limit of no more than 4Gb: it is often 3Gb. Running 32-bit executables on a 64-bit OS will have similar limits: 64-bit executables will have an essentially infinite system-specific limit (e.g., 128Tb for Linux on x86_64 cpus).

4 to 5 GB hard disk is enough to store the system and other important files of a Linux distribution. However, to store users' data it is recommended to have at least 25 GB hard disk size.

Linux requires very little memory to run compared to other advanced operating systems. You should have at the very least 8 MB of RAM; however, it's strongly suggested that you have at least 16 MB. The more memory you have, the faster the system will run.

## What is database?

A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS)

A database is an organized collection of data stored in a computer system and usually controlled by a database management system (DBMS). The data in common databases is modeled in tables, making querying and processing efficient. Structured query language (SQL) is commonly used for data querying and writing.

The Database is an essential part of our life. We encounter several activities that involve our interaction with databases, for example in the bank, in the railway station, in school, in a grocery store, etc. These are the instances where we need to store a large amount of data in one place and fetch these data easily. 

## Applications of mysql?






