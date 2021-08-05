# Basic Commands of MongoDB 

**what is MongoDB?**

MongoDB is an object-oriented, simple, dynamic, and scalable NoSQL database. It is based on the NoSQL document store model. MongoDB created Binary JSON format (BSON) to increase efficiency and support more data types. Data stored in BSON can be searched and indexed, tremendously increasing performance.

**Why use MongoDB?**

1. Makes development easy
2. Stores data in flexible, documents in JSON format
3. Free to use

## Commands that you will use most:
### 1. Login MongoDB
```
mongo -u <username> -p <password> --authenticationDatabase <dbname>
```
### 2. Show all databases
``` 
show dbs
```
### 3. Show collections for the current database
```
 show collections
```
### 4. Create a Collection
```
db.createCollection('collectionName')
```
### 5. Insert a new document to an existing collection
```
db.collectionName.insert(<document>)
```
***Example:*** I want to insert my personal document in family collection -
```
db.family.insert({"Name":"Sifa","Age":22,"Sex":"female"})
```
### 6. Finds a document

=> If you want to find a definite document, then use that command
```
db.collectionName.find(<document>)
```
***Example:***  If you need to find a specific document within a collection by using a field value condition, 
```
db.shop.find({"category":"pen"})
```
=>If you want to find all document, use that
```
db.collectionName.find()
```
### 7. Update a document

If you want to update a specific field of a documnet that matches a given query
```
db.shop.update({"category":"pen"},{"$set":{"subcategory":"Colour-pen"}})
```
Here ``` $set ``` is a query operators. The ```$set``` operator replaces the value of a field with the specified value.
### 8. Remove
```
db..collectionName.remove(<document>)
```
***Example:*** wants to delete a specific field then use,
```
db.shop.remove({"category":"book"})
```
### 9. Count() anad pretty()
count is used to see how many documents are containing a collection and pretty is for showing all data in JSON format.


Check out this [link](https://www.youtube.com/watch?v=Pyk3w_pYPbw) for a practical understanding.