# SQL Cheet Sheet
> learn the thing much faster

##  basic syntax
```
create,insert,update,drop // The most common use in the DB

// create db
create database test ; // create database <DB name>

//list of db
show databases;

// for use the database
use test;//use <DB name>

//create table in DB
create table user // table name
(
  id int primary key
  name varhcar(20) not null
  password varchar(20) not null
);//name of the column data type of the column and how the data type should be

// to store data into the particular data type

insert into user value (1,"username","password"); //This will store the data into the table

//list of the data in the table

select * from user; // show the entire data in the table

select name from user; // this will show the entore name from the table

select * from user limit 2; //this will return a limited value in the table

select * from user limit 2 offset 2; //this link index value return's it skip fist 2 value return 3rd and 4th

select distinct name from user; //this will return the orginal value from table automatically skip the dupilicate value

select count(name) from user; //return count of the data just only a count

select * from user ordered by name; //this will reuturn the data in ordered manner
//Either asc|desc
```

## Using Conditions to filter particular data
```
select * from user where id = 1; //this will return a data that carry id 1;

// Using logical conditions

// AND,OR,NOT

select * from user where id = 1 and name = "username"; // if id 1 and name should be username this will return the data

// =,>,<,>=,<=,<>

select * from user where id > 5; //this will return the data id greater then 5;

// between,like,in

select * from user where between id 5 and 10; //this will return the data based on the id between 5 to 10; all six data will return if exist;
```
