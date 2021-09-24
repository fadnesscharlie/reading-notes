# PostgreSQL

- [Home](https://fadnesscharlie.github.io/reading-notes/401/)

## DataBase

A database is a place where you can store data, change, or delete it. It is stored inside of a server on a comoputer. Most of all the data that is placed on a website comes from a database that they can manipulate.

## SQL

SQL is a programming language. It is a relational database. Been around since 1974.

### Data

Data is stored in tables. This makes it easier to create more rows and colums for each specific data.

## Relational vs Non relational Data base

Relational database will use data from other database that they have a relationship with.

## What is PostgreSQL

- Object-relational Database management system
- Open Source
- Relational database
- Modern

## Postgres Commands

- Create a Database `createdb <Database Name>`
- `/?` or `psql --help` Help for commands
- `/q` Exit command
- `\c <Database Name>` Link to the database after entering `psql`
- `\dt` to see just tables

### Creating your Database Tables

- Make sure to list the type of data type(int, string, VARCHAR, etc)
  - This makes it so that you do not break things when the wrong data is being stored
  - This is a table that we can create using the database name of `test`
  - In here we can see we have `NOT NULL` and `BIGSERIAL`
    - These are some conditions you can put that will say it can not be null, and the id will increment without us having to worry.

`test=# CREATE TABLE person (`  
`test(# id BIGSERIAL NOT NULL PRIMARY KEY,`  
`test(# first_name VARCHAR(50) NOT NULL,`  
`test(# last_name VARCHAR(50) NOT NULL,`  
`test(# gender VARCHAR(7) NOT NULL,`  
`test(# date_of_birth DATE NOT NULL,`  
`test(# email VARCHAR(150) );`

### Adding data to your table

`INSERT INTO person (`  
&nbsp;&nbsp;`first_name,`  
&nbsp;&nbsp;`last_name,`  
&nbsp;&nbsp;`gender,`  
&nbsp;&nbsp;`date_of_birth)`  
`VALUES ('Anne', 'Smith', 'FEMALE', DATE '1988-01-09');`

Below is how it would look when adding it to our database from the terminal

`test=# INSERT INTO person ( first_name, last_name, gender, date_of_birth)` - Press enter to go on a new line
`test-# VALUES ('Anne', 'Smith', 'FEMALE', DATE '1988-01-09');`

We should get a `INSERT 0 1` command proving it worked.



When adding more data to this table, we can just **INSERT** more data. It will create a new ID for us because we used **BIGSERIAL**.

## Other Notes

Postges uses SQL as its main database

## Resources

- [PostGres Youtube Video](https://www.youtube.com/watch?v=qw--VYLpxG4&ab_channel=freeCodeCamp.org)

## Things I want to know more about

-

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
