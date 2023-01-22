# Mongo commands

`show dbs`
`use tucompra`
`db` -> show current db
`db.dropDatabase()` -> Drop database
`db.createCollection("name")` -> Create collection
`show collections`
`db.name.drop()` -> Drop collection
`db.name.insert({})` -> Insert data in the collection (individual)
`db.name.insert({},{})` -> Insert data in the collection (multiple)
`db.name.find().pretty()` -> List all the data
`db.name.update({'name': "Emp1"}, {$set:{'name': 'new emp 1'}})` -> Update data
`db.name.save({"_id": new ObjectId("92349018239"), "name": "Adrian"})` -> Save document
`db.name.remove({"field": "result"})` -> delete document