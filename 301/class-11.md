# In Memory Storage

## Index

[Home](../README.md)  

[SQL and NoSQL](#sql-and-nosql)  
[SQL vs NoSQL (Video)](#sql-vs-nosql-video)

## [SQL and NoSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

### SQL

- `Relational Databases (RDBMS)`
- `table based databases document based`
- `SQL databases have predefined schema`
- `SQL databases are vertically scalable`
- `SQL databases uses SQL ( structured query language ) for defining and manipulating the data`
- `SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL`
- `SQL databases are good fit for the complex query intensive environment`
- `SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server`
- `SQL databases are best fit for heavy duty transactional type applications, as it is more stable and promises the atomicity as well as integrity of the data`
- `Excellent support are available for all SQL database from their vendors. There are also lot of independent consultations who can help you with SQL database for a very large scale deployments.`
- `SQL databases emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability)`
- `On a high-level, we can classify SQL databases as either open-source or close-sourced from commercial vendors.`

### NoSQL

- `Non-relational or distributed database, data in form of tables which consists of n number of rows of data`
- `Key-value pairs, graph databases or wide-column stores or wide-column stores which do not have standard schema definitions`
- `NoSQL databases have dynamic schema for unstructured data`
- `NoSQL databases are horizontally scalable`
- `NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.`
- `NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb`
- `NoSQL databases are not good fit for complex queries`
- `NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.`
- `You can use NoSQL for transactions purpose, it is still not comparable and sable enough in high load and for complex transactional applications.`
- `For some NoSQL database you still have to rely on community support, and only limited outside experts are available for you to setup and deploy your large scale NoSQL`
- `NoSQL database follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance )`
- `NoSQL databases can be classified on the basis of way of storing data as graph databases, key-value store databases, document store databases, column store database and XML databases.`

1. What kind of data is a good fit for an SQL database?
   - SQL databases are good fit for the complex query intensive environment
2. Give a real world example.
   - MySql, Oracle, Sqlite, Postgres and MS-SQL
3. What kind of data is a good fit a NoSQL database?
   - Hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data).
4. Give a real world example.
   - MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb
5. Which type of database is best for hierarchical data storage?
   - NoSQL
6. Which type of database is best for scalability?
Videos
   - SQL altough it seems this is a highly debated topic such as [this quora thread](https://www.quora.com/Why-is-SQL-preferred-over-NoSQL-for-storing-videos-images-and-other-unstructured-data)

## [SQL vs NoSQL (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. What does SQL stand for?
   - Structured Query Language
2. What is a relational database?
   - A [relational database](https://www.oracle.com/database/what-is-a-relational-database) is a type of database that stores and provides access to data points that are related to one another. Relational databases are based on the relational model, an intuitive, straightforward way of representing data in tables. In a relational database, each row in the table is a record with a unique ID called the key. The columns of the table hold attributes of the data, and each record usually has a value for each attribute, making it easy to establish the relationships among data points.
3. What type of structure does a relational database work with?
   - Tables
4. What is a ‘schema’?
   - Product fields, very stric requirments of what fields will be stored in tables. All data has to adhere to the schema, meaning that if a particular data in field A has 6 entries, another data in the same field, field A, can not have 7.
5. What is a NoSQL database?
   - NoSQL database queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language)
6. How does it work?
   - Databases of collections with documentments that can use different fields (no schema).  No relations (kind of).
7. What is inside of a Mongo database?
   - See question 6.  Collections of documents.
8. Which is more flexible - SQL or MongoDB? and why.
   - There is no clear winner. The only place you'll start running into a need to answer this question is when your database is extremely large. Ultimately, it's about what your needs are.  Each has it strengths.  Most companies that need databases use both SQL and NoSQL depending on the problem being solved.
9. What is the disadvantage of a NoSQL database?
   - You must update all collections and may have duplicate data.  Updating info has to be updated in all collections.

[Back To Top](#index)
