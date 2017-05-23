![GitHub Logo](https://s3.ap-south-1.amazonaws.com/greyatom-social/GreyAtom-logo.png)

# Import data into MySQL server

We have provided CSV files within this repo which you need to import in MySQL Server. First thing which we require is to create Database.

## Create Database

You can view all databases in system with below query

    show databases;

You can use below query to create new database. You can create database with any name.

    Create Database greyatom;

## Create Tables

* To import data from CSV we need to create tables first.
* It is required that all tables are created before improting from CSV.
* Follow this tutorial to learn how to create tables. Once you completed with it please come back and start importing data.

## Import Customer table for CSV

* To import CSV we need to keep csv file at perticular location.
* Use below command to get location of upload directory for you mysql installation.

        SHOW VARIABLES LIKE 'secure_file_priv';

* Copy Customers.CSV files to this location.
* Within this repo you will also get script files to import data. Change filepath according to you directory path and execute commands.
* You can see query results in output window. You can also check the content with select statement.

        Select * from greyatom.Customers;

### Case Study
Import data from all given CSV files.

**Notes:**
1. While importing date make sure you are converting from string to date.
2. Handle Null values present in CSV's.
