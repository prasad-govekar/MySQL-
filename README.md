# MySQL-

*Types Of The Database:

1)DDL:(Data Definition Language)
 1.Create
 2.Alter
 3.Drop
 4.Truncate
 5.Rename
 
2)DML:(Data Manipulation Language)
 1.Insert 
 2.Update
 3.Delete
 
3)DCL:(Data Control language)
 1.Grant
 2.Revoke
 
4)TCL:(Transaction Control Language)
 1.Commit 
 2.Rollback
 3.Savepoint

5)DQL(Data Query Language)
 1.Select



----------------------->

1)Create Database is used to create new database
  Syntax: Create database databasename
  
2)Create Command Is Used To create Any Table
  Syntax:Create table stude(Valus)
  
3)Insert is used to insert the data into the table
  Syntax:insert into stude(values)
  
4)To Create table
 create table tabl_name(
 c1_name1 datatype(size),
 c2_name2 datatype(Size),
  .
  .
 c3_name3 datatype(Size).

---------------------->

#Data Types in SQL

1)NUMERIC:
  a.Int-integers
  b.Float-Decimal upto 9 digits
  c.Double-Decimal upto 15 digits
  d.Decimal-decimal fixied
  e.BigInt-Upto 12 digits.
  
2)STRING:
  a.Char-fixed 256
  b.Varchar-varable length
  c.Text-long text
  
3)DATE AND TIME:
  a.Date: yyyy-mm-dd
  b.Datetime: yyyy-mm-dd hh-mm
  c.Time: hh-mm
  d.Timestamp
  e.Year:yyyy

/// Database:
    -Database is collection of data in a format that can be easily accesed (Digital) 
    -A software application used to manage our DB is called Database(Database Management System).

*Two Types of databases:
    1)Relational Database:Data stored in the form of table is called as the relational database.
               -MySQL,SQLSever,ORACLE,PostgreSQL
    2)Non-Relational Database(NoSQL): Data not stored in the form of the table
               -mongoDB
               
*What is SQL?
-Structured Query Language
 SQL is a programming languuage used to interact with relational database
 It is used to perform CRUD opertions:
 Create 
 Read 
 Update
 Delete

*To create database-
        (CREATE DATABASE db_name;)
    Creating our First Table-
     USE db_name;
     CREATE TABLE table_name(
       column1_name1 datatype constraint,
       column2_name2 datatype constraint,
       column3_name3 datatype constraint
       );

*DATATYPES:
     -Most commonly used datatypes:
        1)CHAR
        2)VARCHAR
        3)BLOB
        4)IT
        5)TINYINT
        6)BIGINT
        7)BIT
        8)FLOAT
        9)DOUBLE
        10)BOOLEAN
        11)DATE
        12)YEAR
     -Types Of Datatypes
        1)signed- where we know that both the values can come (positive or negative).
        2)unsigned- Where we know only one type of value can come like (either positive or negative).

*Types of SQL Commands
      1)DDL(data definition language): create, alter, rename, truncate and drop.
      2)DQL(data query language);select.
      3)DML(data manipulation laguage); insert,update and delete.
      4)DCL(data control language);grant and revoke permissions to users.
      5)TCL(transaction control language); start transaction, commit, rollback.

*Database related queries:
      CREATE DATABASE db_name;
      CREATE DATABASE IF NOT EXISTS db_name;
      SAME WITH DROP COMMAND;

      SHOW DATABASE;
      SHOE TABLES;   (*This is called asterics)

*KEYS
1)Primary Keys:(Unique, Not Null)
      -It is a column (or set of columns) in a table that uniquely identifies each row.(a unique id). 
      -There is only 1 PK & it should be NOT NULL.
2)Foreign Keys:
      -A foregin key is a column (or set of columns) in a table that refers to the primary key.
      -There can multiple FKS.
      -FKS can be null and have duplicate values.

*Constraints:
      -SQL constraint are used to specify rules for data in a table.
      -NOT NULL (Columns cannot have a null value || synt: col1 int NOT NULL)
      -UNIQUE (all values in column are different || synt: col2 int UNIQUE)
      -PRIMARY KEY (makes a column unique and not null but used only for one)
      ---->Eg. id int PRIMARY KEY
               CREATE TABLE temp(
               id int NOT NULL,
               PRIMARY KEY(id));

      -FOREGIN KEY (prevets actions that would destroy links between tables
      ------>Eg. CREATE TABLE temp
                 (cust_id int,
                 FOREGIN KEY (cust_id) references customer(id));
            
      
