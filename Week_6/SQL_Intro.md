# Databases
## What is a database?
- A collection of data
- A structured set of data held on a computer
- It can be considered as a container with all the information

Must be able to structure tables to contain the right type of information, so it can be queried

A database can contain multiple tables

A table is displayed in columns and rows
### Terminology
- Column represents a category
    -  Column = database tables are composed of individual columns corresponding to the attributes of the object
- A row contains a collection of data that belongs to one object 
    - Row = a row consists of one set of attributes corresponding to one instance that a table describes, known as a Record

- Table = a table that is predefined format of rows and columns that define an entity, also known as a file

- DBMS = a Database management system allows a computer to perform database functions of storing, retrieving, adding, deleting and modifying data.

### Types of Databases (Db)
- Flat-file Db
  - Stores everything in one Table
  - Good for small numbers of records related toa single topic  
- Relational Db
  - Gives the ability to separate masses of data into numerous tables
  - They are linked to each other through the use of keys (PRIMARY, FOREIGN)  
- big Data
  - Mongo DB, and Vertica use big data
  - Used for Data Analytics and Business Intelligence
  - Digital Age and internet of Things
    
### Relationship Types
- one to one
  - Each row in a table is linked to no more than one row in another table
    - One student may have one row in a contacts table
- one to many
  - Each row in the table can be related to many rows in the relating table
  - allowing for frequently used information to be saved once in a table and referenced many times in all other tables
- many to many
  - One or more rows in a table can be related to 0, 1 or many rows in another table
  - A 3rd table called a mapping or link table is required in order to implement such a relationship
  - For example, customers can purchase many products
  
### Primary key
- It uniquely identifies each record in the table
- Most tables should have a primary key

### Composite key
- Composite is a special form of primary key (not a foreign key)
- Can be made of multiple values/ columns

Constraints: Must be unique, must always have a value, must never change, can only have a maximum number of 1 primary key
### Foreign key
- Used to create solid relationships
- Ensures that the row in table A corresponds to the correct row in table B
- The constraint is used to prevent actions that would destroy links between tables
- It prevents invalid data from being inserted into the foreign key column
- There is no uniqueness Constraint for Foreign keys
- A table can have any number of foreign keys
- A row cannot be deleted from a reference table if it is in via a foreign key