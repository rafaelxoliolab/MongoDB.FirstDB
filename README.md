# First steps with MongoDB
Simple example about first DB on MongoDB.

## MongoDB installation

1. Download setup from [here](https://www.mongodb.com/download-center/community?tck=docs_server).
2. Run the msi file.
3. Install MongoDB as a Windows Service.

## Starting MongoDB Shell
1. Go to `C:\Program Files\MongoDB\Server\4.2\bin`.
2. Double click to `mongo.exe` to open the MongoShell.

## Overview

**Definition**
- MongoDB is a non-SQL database.
- MongoDB is a document oriented database.

**Database**

Database is a physical container for collections.

**Collection**

Collection is a group of MongoDB documents. It is the equivalent of an RDBMS table.

**Document**

A document is a set of key-value pairs. Documents have dynamic schema. 


## Working with MongoDB

Let's start creating next structure:

- **DB**: myfirstdb
  - **Collections**:
    - collectionA
      - **Documents**:
        - documentA1
        - documentA2

1. Create database with `use myfirstdb`.
2. Create collection *collectionA* with `db.createCollection('collectionA')`.
3. Create documents of collectionA with 
  - `db.collectionA.insert(name:"documentA1", description:"this is the documentA1")`
  - `db.collectionA.insert(name:"documentA2", description:"this is the documentA2")`
4. Query documents
  - `db.collectionA.find()`
  - `db.collectionA.find().pretty`

I hope this example helps you as reference in your learning of MongoDB.
