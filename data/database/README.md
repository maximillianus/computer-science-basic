# Database

Here lays the conceptual information about database.

## Database Implementation Layer (RDBMS)
1. Internal/Physical Layer
   1. defines how the data is physically stored.
   2. Related to files, storage method, storage size, indexing method
   3. Example:
      1. index
      2. uses storage definition language
2. Conceptual/Logical Layer
   1. deals with tables and schemas and entity relationship diagram.
   2. referred as **physical data independence** ie. the defined schema is independent of type of RDBMS architecture (physical layer) used
   3. Example:
      1. table
      2. database
      3. schema
      4. uses DDL (Data Definition Language) and DML (Data Manipulation Language)
3. External/View Layer
   1. deals with Views, Reporting, Access Level
   2. referred as **conceptual data independence** ie. the defined View or Report is independent of the underlying ERD, table names (conceptual layer).
   3. Example:
      1. Role Based Access Control
      2. Creating views
      3. uses DDL & VDL (View Definition Language)

## Data Languages
1. DDL
   1. Data Definition Language
   2. Define the database and table structures
   3. Example:
      1. CREATE TABLE
      2. ADD COLUMN
      3. ALTER TABLE
2. DML
   1. Data Manipulation Language
   2. manipulates the data record 
   3. Example:
      1. SELECT
      2. INSERT
      3. UPDATE
3. TCL
   1. Transaction Control Language
   2. Manages the transactions in database
   3. Example:
      1. BEGIN
      2. COMMIT
4. DCL
   1. Data Control Language
   2. Governs the access control for users
   3. Example:
      1. GRANT
      2. REVOKE

## Database Normalization
- 1NF
- 2NF
- 3NF
- BCNF

## Indexing

1. How indexing is done?
   1. [Reference](https://stackoverflow.com/questions/1108/how-does-database-indexing-work#:~:text=Indexing%20is%20a%20way%20of,to%20be%20performed%20on%20it.)
2. Clustered vs Non-clustered index?
   1. [Reference](https://medium.com/fintechexplained/clustered-vs-non-clustered-index-8efed55ed7b9)
   2. Clustered:
      1. What:
         1. Index which physically orders the data
         2. Ex: Primary Key
         3. stored as trees which contains actual data in the nodes
         4. Used to improve data retrieval performance
      2. How:
         1. Create primary key
      3. When:
         1. When order is needed
         2. When filtering on specific columns
         3. When trying to read a lot of data
   3. Non-Clustered:
      1. What:
         1. logical ordering of data.
         2. Ex: common index
         3. storing pointers instead of all data
         4. Use on columns needed to join table to improve performance
      2. How:
         1. create normal index ie. `CREATE INDEX`
         2. create non-clustered index ie. `CREATE NON-CLUSTERED INDEX`
      3. When:
         1. When order is needed
         2. When filtering on different columns
         3. when doing custom indexing

## Data Dictionary

1. Best Practice for creating Data Dictionary
   1. start small & iterate
   2. version control (google spreadsheet & github wiki can version control)
   3. Consider who is your audience, build dictionary that fits the audience


## NoSQL Database
There are 4 types of NoSQL Database.
1. Columnar
   1. Use Cases:
      1. OLAP - analytics
   2. Example:
      1. Open Source: Cassandra, HBase
      2. Cloud: AWS Keyspaces
2. Document
   1. Use Cases:
      1. flexible schema app
      2. content management
   2. Example:
      1. Open Source: MongoDB
      2. Cloud: AWS DocumentDB, AWS DynamoDB
3. Key-Value
   1. Use Cases:
      1. caching
      2. session management
   2. Example:
      1. Open Source: Redis, Memcache
      2. Cloud: AWS ElastiCache, AWS DynamoDB
4. Graph
   1. Use Cases:
      1. fraud detection
      2. social networking
   2. Example:
      1. Open Source: Neo4J
      2. Cloud: AWS Neptune

