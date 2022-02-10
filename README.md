-# SQL_assigment1<br>


testdb=# \q<br>
temporaryadmin@C02G10CXML86 ~ % createdb "Digital Career Institute"<br>
temporaryadmin@C02G10CXML86 ~ % psql "Digital Career Institute" <br>


Digital Career Institute=# \q<br>

temporaryadmin@C02G10CXML86 ~ % psql<br>

temporaryadmin=# ALTER DATABASE "Digital Career Institute" RENAME TO dci;<br>


temporaryadmin-# \q<br>
temporaryadmin@C02G10CXML86 ~ % psql dci<br>


dci=# SELECT current_schema();
 current_schema 
----------------
 public
(1 row) <br>


dci=# SHOW search_path;
   search_path   
-----------------
 "$user", public
(1 row) <br>


dci=# CREATE SCHEMA students;
CREATE SCHEMA <br>
dci=# CREATE SCHEMA courses;
CREATE SCHEMA<br>
dci=# CREATE SCHEMA partners;
CREATE SCHEMA<br>
dci=# CREATE SCHEMA sales;
CREATE SCHEMA<br>

**CREATE TABLE**

dci=# CREATE TABLE students.java(. <br>
dci(# name varchar (50),   <br>
dci(# active boolean, <br>
dci(# startDate date);  <br>

CREATE TABLE
dci=# CREATE TABLE students.python(. <br>
dci(# name varchar (50), <br>
dci(# active boolean, <br>
dci(# startDate date); <br>

CREATE TABLE
dci=# CREATE TABLE courses.frontEnd(<br>
dci(# name varchar (50),<br>
dci(# duration int);<br>

CREATE TABLE
dci=# CREATE TABLE courses.backEnd(<br>
dci(# name varchar (50),<br>
dci(# duration int);<br>

CREATE TABLE
dci=# CREATE TABLE partners.company(<br>
dci(# name varchar (50),<br>
dci(# city varchar (50));<br>

CREATE TABLE
dci=# CREATE TABLE partners.sales(<br>
dci(# department varchar (50),<br>
dci(# employees int);<br>

dci=# SET search_path TO courses, public;
SET


**INSERT INTO**<br>
dci=# INSERT INTO backend VALUES ('Java', '12'), ('Python', '10'),('JavaScript','8');
INSERT 0 3

**CREATE INFO**<br>
dci=# CREATE TABLE sales.department();
CREATE TABLE

**REMOVE INfO**<br>
dci=# DROP TABLE sales.department;
DROP TABLE

**INSERT INTO**<br>
dci=# INSERT INTO students.java VALUES ('Anna', 'no', '1990-01-01'), ('Klaus', 'yes','2021-09-09');
INSERT 0 2

**TRUNCATE --> truncate means remove only the data in the table, not the table**<br>
dci=# TRUNCATE TABLE students.java;
TRUNCATE TABLE

**RENAME TABLE**<br>
dci=# ALTER TABLE partners.sales RENAME TO creditControl;
ALTER TABLE
dci=# 
