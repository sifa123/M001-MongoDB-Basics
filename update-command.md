You can update document in three ways- update(), updateOne(), updateMany(). Let's see some examples of them

### 1. update()
```
db.collectionName.update(<document>)
```
***Example:***  By using update method, you can update single document. Here I will show you upating a single document named shop_address
```
db.shop.update({"shop_address":"Bangladesh"},{$set:{"shop_address":"USA"}})
```
The `$set` works for update, it will replace shop_address from Bangladesh to USA.

### 2. updateOne()
```
db.collectionName.updateOne(<document>)
```
***Example:*** By using updateOne command, you can update only a single document.
```
db.shop.updateOne({"shop_address":"Bangladesh"},{$set:{"shop_address":"USA"}})
```
### 3. updateMany()
```
db.collectionName.updatemany(<document1>,<document2>,...)
```
***Example:***
```
db.shop.updateMany({"shop_num":{"$gt":"10"}},{"$set":{"shop_num":"5"}})
```
#### The main difference among them are-

**updateMany() :** It update all documents in a collection with matching filter.

**updateOne() :** It update only one top most document in a collection with matching filter.

**update() :** By default, the update() method updates a single document.

You can clear your doubts by seeing this [video](https://www.youtube.com/watch?v=fnw6qYwohmQ). 