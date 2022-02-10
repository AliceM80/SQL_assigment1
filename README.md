-# SQL_assigment1


testdb=# \q
temporaryadmin@C02G10CXML86 ~ % createdb "Digital Career Institute"
temporaryadmin@C02G10CXML86 ~ % psql "Digital Career Institute" 


Digital Career Institute=# \q

temporaryadmin@C02G10CXML86 ~ % psql

temporaryadmin=# ALTER DATABASE "Digital Career Institute" RENAME TO dci;
ALTER DATABASE

temporaryadmin-# \q
temporaryadmin@C02G10CXML86 ~ % psql dci
psql (14.1)
Type "help" for help.

dci=# SELECT current_schema();
 current_schema 
----------------
 public
(1 row)

dci=# SHOW search_path;
   search_path   
-----------------
 "$user", public
(1 row)


dci=# CREATE SCHEMA students;
CREATE SCHEMA
dci=# CREATE SCHEMA courses;
CREATE SCHEMA
dci=# CREATE SCHEMA partners;
CREATE SCHEMA
dci=# CREATE SCHEMA sales;
CREATE SCHEMA

**CREATE TABLE**

dci=# CREATE TABLE students.java(. <br>
dci(# name varchar (50),   <br>
dci(# active boolean, <br>
dci(# startDate date);  <br>

CREATE TABLE
dci=# CREATE TABLE students.python(
dci(# name varchar (50),
dci(# active boolean,
dci(# startDate date);
CREATE TABLE
dci=# CREATE TABLE courses.frontEnd(
dci(# name varchar (50),
dci(# duration int);
CREATE TABLE
dci=# CREATE TABLE courses.backEnd(
dci(# name varchar (50),
dci(# duration int);
CREATE TABLE
dci=# CREATE TABLE partners.company(
dci(# name varchar (50),
dci(# city varchar (50));
CREATE TABLE
dci=# CREATE TABLE partners.sales(
dci(# department varchar (50),
dci(# employees int);
CREATE TABLE

dci=# SET search_path TO courses, public;
SET


**INSERT INTO**
dci=# INSERT INTO backend VALUES ('Java', '12'), ('Python', '10'),('JavaScript','8');
INSERT 0 3

**CREATE INFO**
dci=# CREATE TABLE sales.department();
CREATE TABLE

**REMOVE INfO**
dci=# DROP TABLE sales.department;
DROP TABLE

**INSERT INTO**
dci=# INSERT INTO students.java VALUES ('Anna', 'no', '1990-01-01'), ('Klaus', 'yes','2021-09-09');
INSERT 0 2

**TRUNCATE --> truncate means remove only the data in the table, not the table**
dci=# TRUNCATE TABLE students.java;
TRUNCATE TABLE

**RENAME TABLE**
dci=# ALTER TABLE partners.sales RENAME TO creditControl;
ALTER TABLE
dci=# 
