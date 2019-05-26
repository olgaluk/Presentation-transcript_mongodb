# Presentation-transcript_mongodb
Hello, my name is Olga. Today I want to present you my report about the mongoDB database.

Let's start with the definition.

**MongoDB** is a NoSQL database which stores the data in form of key-value pairs. It is an Open Source, Document Database which provides high performance and scalability.

**What is Document based storage?**

A Document is nothing but a data structure with name-value pairs like in JSON.
The values of fields may include other documents, arrays, and arrays of documents.

**History of MongoDB**

MongoDB was developed by Eliot Horowitz and Dwight Merriman in the year 2007, when they experienced some scalability issues with the relational database while developing enterprise web applications at their company DoubleClick.
In 2009, MongoDB was made as an open source project.
In 2013, the company was officially named to MongoDB Inc.

**Organizations that use MongoDB**

Below are some of the big and notable organizations which are using MongoDB as database for most of their business applications.
 -	Adobe
 -	FourSquare
 -	eBay
 -	MetLife
 -	SAP

**Features of MongoDB**

1.	MongoDB provides high performance. Most of the operations in the MongoDB are faster compared to relational databases.
2. MongoDB provides auto replication feature that allows you to quickly recover data in case of a failure.
3. Horizontal scaling is possible in MongoDB because of sharing. Sharing is partitioning of data and placing it on multiple machines in such a way that the order of the data is preserved.
4. Load balancing: Horizontal scaling allows MongoDB to balance the load.
5. High Availability: Auto Replication improves the availability of MongoDB database.
6. Indexing: Index is a single field within the document. Indexes are used to quickly locate data without having to search every document in a MongoDB database. This improves the performance.

**Overview of MongoDB**

MongoDB consists of a set of databases. Each database again consists of Collections. Data in MongoDB is stored in collections. This slide shows the typical database structure in MongoDB.
Database in MongoDB is nothing but a container for collections.
Collection is nothing but a set of MongoDB documents.
Document in MongoDB is nothing but the set of key-value pairs.
Remember, the value of fields in a document can be anything, including other documents, arrays, and arrays of documents.

**Database Create and Drop**

Let's see how to create the database.
The “use” command helps us to create a database. 
This will create a new database with the name database_name if there is no database already present with the same name. If a database already exists with the same name, then it just connects to that database.
Now let's see how to remove the database.
First check the list of databases available, using the show dbs command.
If the newly created database database_name has to be dropped(deleted), run “dropDatabase” command to delete the database. Before deleting the database, connect to the required database which is to be deleted.

**Collection Create and Drop**

In MongoDB a collection is automatically created when it is referenced in any command. For example, if you run an insert command : “db.student.insert”.
Above command will create a collection named student if it doesn't exist already in the database. But we can explicitly create a collection using the createCollection() command. 
Any collection in a database in MongoDB can be dropped easily using the following command: “db.collection_name.drop”.
drop() method will return true is the collection is dropped successfully, else it will return false.

**CRUD Operations in MongoDB**

CRUD operations refer to the basic Insert, Read, Update and Delete operations. Now, let us learn how to perform CRUD (Create/Read/Update/Delete) operations in MongoDB.
The command db.collection.insert() will perform an insert operation into a collection of a document.
To Select the inserted document, run “db.collection_name.find” command. The find() command will retrieve all the documents of the given collection.
If a record is to be retrieved based on some criteria, the find() method should be called passing parameters, then the record will be retrieved based on the attributes specified.
In order to update specific field values of a collection in MongoDB, run “db.collection_name.update” query.
update() method specified above will take the fieldname and the new value as argument to update a document.
Let us now look into the deleting an entry from a collection. In order to delete an entry from a collection, run the command “db.collection_name.remove”.

We reviewed the basics of working with this database. Thank you for attention.

