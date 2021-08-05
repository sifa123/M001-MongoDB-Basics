MQL is an SQL-like query engine tailored for MongoDB, giving you the performance of native queries with the productivity of SQL.
We can say that in MongoDB, there are about five operators but we will discuss only three operators- update, query and logic operator.
### 1. Update Operators
**$inc:** Increments the value of the field by the specified amount. 

**$set:** Increments the value of the field by the specified amount.

**$unset:** Removes the specified field from a document.

**$min:** Only updates the field if the specified value is less than the existing field value.

**$max:** Only updates the field if the specified value is greater than the existing field value.

### 2. Query Operators
**$eq:** Matches values that are equal to a specified value.

**$gt:** Matches values that are greater than a specified value.

**$gte:** Matches values that are greater than or equal to a specified value.

**$in:** Matches any of the values specified in an array.

**$lt:** Matches values that are less than a specified value.

**$lte:** Matches values that are less than or equal to a specified value.

**$ne:** Matches all values that are not equal to a specified value.

**$nin:** Matches none of the values specified in an array.

### 3. Logic Operator
**$and:** Match all of the specified query clauses.

**$or:** At least one of the query clauses is matched.

**$nor:** Fail to match given clauses.

**$not:** Negates the query requirement.