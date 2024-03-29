# MySql_Tutorial
This is open book for everyone to learn add and edit the contents all about mysql

Welcome to this open book on **"Learn Everything About Mysql"**. 

I am **Amit Kumar Sah**, and I have two years of programming experience. 

I love Programming. One of the aims I had when I started Writing this was to make learning mysql easy. 

In this book, you will learn to write **queries** **concepts of mysql**. You will be exposed to a lot of examples, exercises and tips. We will take up a lot of examples, and try and see how to write mysql queries. 

Help us improve this guide - **Fork, Pull Requests, Shares and Likes are recommended**!


## Table of Contents

* [Chapter 01 - MySQL Getting Started](#MySQL-Getting-Started)
    * [About MySQL](#About-MySQL)
    * [Download Sample Database](#download-sample-database)
    * [Load Sample Database in MySQL](#load-sample-database)
* [Chapter 02 - Data Manipulation in MySQL](#data-manupulation-in-mysql)
    * [select Query in MySQL](#select-query-in-mysql)
   
    
    
    
## MySQL Getting Started
### About MySQL
#### What Is MySQL and Why It Is the World’s Most Popular Open Source Database

> Summary: this tutorial helps you answer the question: what is MySQL? And give you the reasons why MySQL is the world’s most popular open source database.

To understand MySQL, you need to understand database and SQL first. If you already know database and SQL, you can jump to the What is MySQL section.

##### Introduction to database

You deal with data every day…

When you want to listen to your favorite songs, you open your playlist from your smartphone. In this case, the playlist is a database.

When you take a photo and upload it to your account on a social network like Facebook, your photo gallery is a database.

When you browse an e-commerce website to buy shoes, clothes, etc., you use the shopping cart database.

Databases are everywhere. So what is a database?  By definition, a database is merely a structured collection of data.

The data relate to each other by nature, e.g., a product belonged to a product category and associated with multiple tags. Therefore, we use the term relational database.

In the relational database, we model data like products, categories, tags, etc., using tables. A table contains columns and rows. It is like a spreadsheet.

A table may relate to another table using a relationship, e.g., one-to-one and one-to-many relationships.

Because we deal with a significant amount of data, we need a way to define the databases, tables, etc., and process data more efficiently. Besides, we want to turn the data into information.

And this is where SQL comes to play.
SQL – the language of database

SQL stands for structured query language.

SQL is the standardized language used to access the database.

> ANSI/SQL defines the SQL standard. The current version of SQL is SQL:2003. Whenever we refer to the SQL standard, we mean the current SQL version.

SQL contains three parts:

    Data definition language(DDL) includes statements that help you define the database and its objects, e.g., tables, views, triggers, stored procedures, etc.
    Data manipulation language(DML) contains statements that allow you to update and query data.
    Data control language(DCL) allows you to grant the permissions to a user to access specific data in the database.

Now, you understand database and SQL, and it’s time to answer the next question…

What is MySQL?

My is the daughter’s name of the MySQL’s co-founder, Monty Widenius.

The name of MySQL is the combination of My and SQL, MySQL.

MySQL is a database management system that allows you to manage relational databases. It is open source software backed by Oracle. It means you can use MySQL without paying a dime. Also, if you want, you can change its source code to suit your needs.

Even though MySQL is open source software, you can buy a commercial license version from Oracle to get a premium support services.

MySQL is pretty easy to master in comparison with other database software like Oracle Database, or Microsoft SQL Server.

MySQL can run on various platforms UNIX, Linux, Windows, etc. You can install it on a server or even in a desktop. Besides, MySQL is reliable, scalable, and fast.

>The official way to pronounce MySQL is My Ess Que Ell, not My Sequel. However, you can pronounce it whatever you like, who cares?

If you develop websites or web applications, MySQL is a good choice. MySQL is an essential component of LAMP stack, which includes Linux, Apache, MySQL, and PHP.

### Download Sample Database
You can download sample database used for examples from [here](https://dev.mysql.com/doc/index-other.html) or from same github repository.

you can download description abot the database from [here](https://dev.mysql.com/doc/sakila/en/sakila-authors-note.html)


### Load Sample Database in MySQL
To load database through command line in linux operating environment.
```sql

[amitsa-dt@amitsa]$ mysql -uroot -ppassword
mysql: [Warning] Using a password on the command line interface can be insecure.
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 1041
Server version: 5.7.22-enterprise-commercial-advanced-log MySQL Enterprise Server - Advanced Edition (Commercial)

Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| database           |
| mysql              |
| nmsdb              |
| performance_schema |
| sys                |
| tejnmsdb           |
+--------------------+
7 rows in set (0.00 sec)

mysql> create database sakila;
Query OK, 1 row affected (0.00 sec)

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| database           |
| mysql              |
| nmsdb              |
| performance_schema |
| sakila             |
| sys                |
| tejnmsdb           |
+--------------------+
8 rows in set (0.00 sec)

##To Load schema and data in sakila database
[amitsa-dt@amitsa sakila-db]$ mysql -uroot -pIltwat@1 sakila < sakila-schema.sql
mysql: [Warning] Using a password on the command line interface can be insecure.
[amitsa-dt@amitsa sakila-db]$ mysql -uroot -pIltwat@1 sakila < sakila-data.sql
mysql: [Warning] Using a password on the command line interface can be insecure.
```
## select Query in MySQL




