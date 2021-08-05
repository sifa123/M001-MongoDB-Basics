By using delete method in MongoDB, you can remove or delete any collections or documents which are exists in your MongoDB collections. Just like update,insert command there two types of command in delete- deleteOne(), deleteMany()

### 1. deleteOne()
```
db.collectionName.deleteOne(<document>)
```
***Example:*** What you will declare in this bracket, only single document that will be delted if it exists in your collection.
```
db.shop.deleteOne({"owner_name":"Sifa"})
```
Here if any owner_name with Sifa matches then, this(single document) will be deleted.

### 2.deleteMany()
```
db.shop.deleteMany(<document>)
```
***Example:*** In this example I have mentioned an owner_name, Sifa. If it is macthed with any document like 10 or 30 all of them will be deleted which are named(owner_name) with Sifa. 
```
db.shop.deleteMany({"owner_name":"Sifa"})
```
Check out this [link](https://www.youtube.com/watch?v=OeoOWwZ1k9I) for details.