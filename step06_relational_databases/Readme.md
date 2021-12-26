# Step06 - Learning Relational Databases

## Class Notes

Relational databases are the oldest one and they have a major issue of not being scaleable. Then documnet databases became teh norm, MangoDb was one of them but they have the problem of designing robust database. As database is constructed based on queries and if new queries arises there is lot difficulty to handle. Now there is development of distributed relational databases. Now we have the option of SQL distributed relational databases whihc are also scalebale. When there is lot of relations between the data Graph Databases are to be used. When there is very simple project document database can be used. For the complex apps with less connection between the data relational databases are the best.

- [Relational Databases Design](https://www.guru99.com/database-design.html)

  - What is Database Design
    - Sketching and planning part of the designing and implementation is part of development.
    - Database design helps with the designing, development, implementation and maintainance. It is important to decide how data elements corelate and what data to be stored. Major objective is to produce logical and physical designs models.
    - Logical model is about data requirement and data to be stored. (id of some product to store)
    - Physical model is about logical DB design and about physical media. (specifications of the id)
  - Database development life cycle
    - Requirements analysis
      - Planning - concerned with the planning of the entire database devlopment cycle
      - System defination - define scope and boundries
    - Database designing
      - Logical Model
      - Physical model
    - Implementation
      - data conversion - importing and converting old data
      - testing
  - Two Types of Database Techniques
    - Normalization
    - ER Modeling

- [What is Normalization](https://www.guru99.com/database-normalization.html)
  - Normalization is to reduces data redundancy and eliminates undesirable characteristics it divides larger tables into smaller tables and links them using relationships.
  - KEYs in SQL? - Key is for identifying a record uniquely. It can be a single or multiple columns used to identify rows. It is also used for finding duplicate data or making relations. And columns other than keys are known as non key columns.
    - Primary Key - A primary is a single column value used to identify a database record uniquely. It should have following properties
      - A primary key cannot be NULL
      - A primary key value must be unique
      - The primary key values should rarely be changed
      - The primary key must be given a value when a new record is inserted.
    - Composite Key
  - Database Normal Forms - 3rd normal form is considered the best
    - 1NF (First Normal Form)
    - 2NF (Second Normal Form)
    - 3NF (Third Normal Form)
    - BCNF (Boyce-Codd Normal Form)
    - 4NF (Fourth Normal Form)
    - 5NF (Fifth Normal Form)
    - 6NF (Sixth Normal Form)
  - 1NF (First Normal Form) Rules
    - Each table cell should contain a single value.
    - Each record needs to be unique.
