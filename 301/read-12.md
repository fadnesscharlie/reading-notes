# Mongo and Mongoose

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

Reading
## nosql vs sql

### Fill in the chart below with five differences between SQL and NoSQL databases:

<table style="width:100%">
  <tr>
    <th>SQL</th>
    <th>NoSQL</th> 
  </tr>
  <tr>
    <td>Data uses Schemas</td>
    <td>Schema-less</td>
  </tr>
  <tr>
    <td>Relations</td>
    <td>No (or very few) Relations</td>
  </tr>
  <tr>
    <td>Data is ditributed across multiple tables</td>
    <td>Data is typically merged/nested ina a few collections</td>
  </tr>
  <tr>
    <td>Horizontal scaling is difficult/impossible;
    Vertical scaling is possible</td>
    <td>Both horizontal and vertical scaling is possible</td>
  </tr>
  <tr>
    <td>Limitations for lots of (thousands)
     read & write queries per second</td>
    <td>Great performance for mass (simple) read & write requests</td>
  </tr>
</table>
 	 
 	 
1. What kind of data is a good fit for an SQL database?
   1. Data that is very specific and new values are updated for the new data it takes in
2. Give a real world example.
   1. Account based data
3. What kind of data is a good fit a NoSQL database?
   1. More static data, which does not have a lot of relations.
   2. Read/Write a lot but not updating a lot.
4. Give a real world example.
   1. Survey Data
5. Which type of database is best for hierarchical data storage?
   1. SQL
6. Which type of database is best for scalability?
   1. SQL

## sql vs nosql (Video)

1. What does SQL stand for?
   1. Structured Query Language
2. What is a relational database?
   1. How different tables relate to one another.
   2. Updates one information to other tables when making new data
3. What type of structure does a relational database work with?
   1. Vertical Scaling
4. What is a ‘schema’?
   1. A predictable layout
5. What is a NoSQL database?
   1. A data base that is less strict then SQL.
6. How does it work?
   1. Works with horizontal or vertical scaling but does not have good relations
7. What is inside of a Mongo database?
   1. JSON formatted Data
8. Which is more flexible - SQL or MongoDB? and why.
   1. MongoDB is more flexiable because it is more flexiable with
9. What is the disadvantage of a NoSQL database?
   1. Relations and updating data constantly

## Resources

- [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

## BookMark/Skim

- [mongoose api](https://mongoosejs.com/docs/api.html#Model)
- [sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

## Things I want to know more about

- How to grab from a database, implementing it, and possibly changing the database.

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
