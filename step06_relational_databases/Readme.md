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
    - Composite Key - A composite key is a primary key composed of multiple columns used to identify a record uniquely
    - Foreign Key - Foreign Key references the primary key of another Table! It helps connect your Tables - You will only be able to insert values into your foreign key that exist in the unique key in the parent table. This helps in referential integrity.
      - A foreign key can have a different name from its primary key
      - It ensures rows in one table have corresponding rows in another
      - Unlike the Primary key, they do not have to be unique. Most often they aren’t
      - Foreign keys can be null even though primary keys can not
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
  - 2NF (Second Normal Form) Rules
    - Be in 1NF
    - Single Column Primary Key that does not functionally dependant on any subset of candidate key relation
  - 3NF (Third Normal Form) Rules
    - Be in 2NF
    - Has no transitive functional dependencies - A transitive functional dependency is when changing a non-key column, might cause any of the other non-key columns to change
  - BCNF (Boyce-Codd Normal Form)
    - Even when a database is in 3rd Normal Form, still there would be anomalies resulted if it has more than one Candidate Key.
  - 4NF (Fourth Normal Form) Rules
    - If no database table instance contains two or more, independent and multivalued data describing the relevant entity, then it is in 4th Normal Form.
  - 5NF (Fifth Normal Form) Rules
    - A table is in 5th Normal Form only if it is in 4NF and it cannot be decomposed into any number of smaller tables without loss of data.
  - 6NF (Sixth Normal Form) Proposed

- [What is ER Modeling](https://www.guru99.com/er-modeling.html)
  - Entity Relationship is a graphical approach to database design. It defines data elements and their relationship.
  - An Entity is a thing or object in real world that is distinguishable from surrounding environment
    - An entity has a set of properties
    - Entity properties can have values.
  - Entities can have relationships.
  - Enhanced Entity Relationship (EER) Model
    - EER Model is a high-level data model which provides extensions to original ER model. EER Models supports more details design. EER Modeling emerged as a solution for modeling highly complex databases.
    - EER uses UML notation.
      - Entities are represented as class diagrams.
      - Relationships are represented as associations between entities.
  - Why use ER Model?
    - Relational DB dont support many to many reltaions
