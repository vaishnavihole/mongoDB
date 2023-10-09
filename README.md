### MongoDB commands for Databases

1. **View all databases**
   - Command: `show dbs`
   - Description: This command displays a list of all the databases available in your MongoDB server.

2. **Create a new or switch database**
   - Command: `use dbName`
   - Description: You can use this command to create a new database with the specified name or switch to an existing database with the given name.

3. **View current database**
   - Command: `db`
   - Description: This command shows you the name of the currently selected database.

4. **Delete database**
   - Command: `db.dropDatabase()`
   - Description: Use this command to delete the currently selected database along with all its collections and data.

### MongoDB commands for Collections

5. **Show Collections**
   - Command: `show collections`
   - Description: This command lists all the collections within the currently selected database.

6. **Create a collection**
   - Command: `db.createCollection(collectionName)`
   - Description: You can use this command to create a new collection with the specified `collectionName` within the current database.

7. **Delete Collection**
   - Command: `db.collectionName.drop()`
   - Description: This command deletes the collection with the specified `collectionName` from the current database.

### MongoDB commands for Rows (Documents)

8. **Insert One Row**
   - Command: `db.collectionName.insert({})`
   - Description: Use this command to insert a single document (row) into the specified collection with empty data. You can replace the `{}` with the data you want to insert.

9. **Insert Many Rows**
   - Command: `db.collectionName.insertMany([{}])`
   - Description: This command allows you to insert multiple documents (rows) into the specified collection with the provided data. You can insert an array of objects containing the data.

10. **Show all Rows in Collection**
    - Command: `db.collectionName.find()`
    - Description: This command retrieves and displays all the documents (rows) within the specified collection.

11. **Find the first row matching the object**
    - Command: `db.collectionName.findOne({key: 'value'})`
    - Description: It retrieves and returns the first document in the collection that matches the specified criteria (`key: 'value'`).

12. **Show all Rows in Collection (Prettified)**
    - Command: `db.collectionName.find().pretty()`
    - Description: This command displays all the documents in the collection in a more human-readable, formatted manner.

13. **Search in MongoDB Database**
    - Command: `db.collectionName.find({key: 'value'})`
    - Description: Use this command to search for documents in the collection that match the specified criteria (`key: 'value'`).

14. **Limit the number of rows in output**
    - Command: `db.collectionName.find().limit(number)`
    - Description: It limits the number of documents returned in the output to the specified `number`.

15. **Count the number of rows in the output**
    - Command: `db.collectionName.find().count()`
    - Description: This command counts and returns the total number of documents in the collection that match the query criteria.

16. **Update a document**
    - Command: `db.collectionName.update({key: 'value'}, {$set: {key: 'updated value'}})`
    - Description: Use this command to update a document in the collection that matches the specified criteria by setting a new value for a specific key.

17. **MongoDB Increment Operator**
    - Description: The provided JavaScript code demonstrates how to use the MongoDB Increment Operator to increment the value of a key within a document.

18. **MongoDB Rename Operator**
    - Description: The provided JavaScript code demonstrates how to use the MongoDB Rename Operator to rename a key within a document.

19. **Delete Row**
    - Command: `db.collectionName.remove({key: 'value'})`
    - Description: This command allows you to delete documents in the collection that match the specified criteria (`key: 'value'`).