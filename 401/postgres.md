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
`test(# country_of_birth NOT NULL,`  
`test(# email VARCHAR(150) );`

### Adding data to your table

`INSERT INTO person (`  
&nbsp;&nbsp;`first_name,`  
&nbsp;&nbsp;`last_name,`  
&nbsp;&nbsp;`gender,`  
&nbsp;&nbsp;`date_of_birth)`
&nbsp;&nbsp;`country_of_birth)`  
`VALUES ('Anne', 'Smith', 'FEMALE', '1988-01-09', 'France');`

Below is how it would look when adding it to our database from the terminal

`test=# INSERT INTO person ( first_name, last_name, gender, date_of_birth, country_of_birth)` - Press enter to go on a new line
`test-# VALUES ('Anne', 'Smith', 'FEMALE','1988-01-09', 'France');`

We should get a `INSERT 0 1` command proving it worked.

When adding more data to this table, we can just **INSERT** more data. It will create a new ID for us because we used **BIGSERIAL**.

## Running a file with SQL data

When you want to run a file, say import it inside of your postgres database, we can use the command `\i <filepath>`. This will run whatever is in that file. It can be to create a whole new table, or it can be to add files to an exsisting table.

## SELECT, sort, etc Command

- `SELECT * FROM <databaseName>;` will print out your current database to see what is **all** inside
  - Ex. `SELECT gender FROM person;`
    - Returns only gender from the table person
- `SELECT first_name, last_name, <parameter from table> FROM person;` will print out all of the first and last names along with what other table header you want in your database.
- Selecting no parameters returns back just the rows.
- `SELECT * FROM <database> ORDER BY <parameter(example would be date_of_birth)>;`
  - This will print out our data in ascending order.
    - This works for date, numbers, and strings.
  - Example:
    `SELECT * FROM person ORDER BY date_of_birth ASC;` will filter by ascending order
    `SELECT * FROM person ORDER BY date_of_birth DESC;` will filter by descending order
- `SELECT DISTINCT first_name FROM person ORDER BY first_name;`
  - This will return the first names of people, but no repeating names and sort them for us.'
- `SELECT * FROM person WHERE gender = 'Female';`
  - This will return back data from only data that has 'Female'
- `SELECT * FROM person WHERE gender = 'Female' AND (first_name = 'Jennifer' OR first_name = 'Sarah');`
  - We can sort even further to get only females named Jennifer
    - We can add parentheses around a conditional to sort by more variables

## Comparison Operators

- `SELECT 1 = 1;`
  - This will return either a `t` or `f` for true or false.
- The operator can be used for `=`, `<=`, and even `<>` for not true
- You can compare them between data and not just numbers.

## Limit, Offset, and Fetch

- You can select which rows you want to see with Limit and Offset.
  - In doing so, you would have to use `SELECT * FROM person LIMIT 5;`
    - This will show only the first 5.
  - `SELECT * FROM person OFFSET 5 LIMIT 5;`
    - This will return ropws 6-10.
  - Using variations you can use Offset and Limit by itself
- More of SQL standard would be to use Fetch.
  - `SELECT * FROM person OFFSET 5 FETCH FIRST <num/blank for first> ROW ONLY;`
    - This will return rows 6 - whatever number you declare after 6.
      - Example would be:
        - `SELECT * FROM person OFFSET 5 FETCH FIRST 10 ROW ONLY;`
          - You will get the rows between 5 and 15

## In

- Instead of using `SELECT * FROM person WHERE country_of_birth = 'France' OR country_of_birth = 'Brazil' OR country_of_birth = 'China'`
  - You can short hand this to `SELECT * FROM person WHERE country_of_birth IN ('China', 'Brazil', 'France')`

## Between

- You can select between two things, especially for our `date_of_birth`
  - `SELECT * FROM person WHERE date_of_birth BETWEEN DATE '2000-01-01' AND '2015-01-01'`
    - We will see all people who were born between 2000 and 2015.

## Other Notes

- Postges uses SQL as its main database
- Make sure you use your `;`, it is very important as it says when to stop.

## Resources

- [PostGres Youtube Video](https://www.youtube.com/watch?v=qw--VYLpxG4&ab_channel=freeCodeCamp.org)

## Things I want to know more about

-

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
