# MongoDB: noSQL database

General schema:
- Databaseses --> collections --> documents
- Each document within the colleciton is one JSON object. The documents may have nested info, do not have to have matching fields/sizes, etc

[Install set up via github README](https://github.com/mongodb/homebrew-brew)

commands:  
- To start mongoDB:
- `brew services start mongodb-community`  
- To connet to mongoDB shell: `mongosh`
- To get out of mongoDB shell: `ctrl + C` twice, or `exit`
- To get out of mongoDB: `brew services stop mongodb-community`
---

## Commands within MongoDB shell:

- show all databases:
`show dbs`
  Connect to a database:
`use <database_name:new_or_existing>` 
 
- To show data within a database:
`show collections` 

- To see data within a collection:
`db.<collection_name>.find()`

- To delete a database:
`db.dropDatabase()` 
(response: `{ ok: 1, dropped: 'practicedb' }`)

clear screen: `cls`

- To add one document to the collection:  
 `db.<collection_name>.insertOne({json_object})`
Example:
```
practicedb> db.users.insertOne({name: "Jenny"})
{
  acknowledged: true,
  insertedId: ObjectId("62dad8399ecac24b878b12da")
}
practicedb> 
```
- To add multiple documents to a collection:   Add an array of objects:  

`db.<collection_name>.insertMany([{json_obj1}, {json_obj2}])`
