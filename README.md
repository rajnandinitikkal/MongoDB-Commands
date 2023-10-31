# MongoDB Commands

## MongoDB CRUD Operations

- Displays a list of all available database in MongoDB instance.
```
show dbs
```

- Switches to the specified database , making it the active database for subsequent operations.
```
<db name>
```
[screenshot](./Output/Usedb.png)

- Inserta a single document into a mangoDB collection.
```
insertOne()
```
```
db.courses.insertOne({
    title: 'IGCP-1.0',
    description: 'Full stack web development',
    fees: 15000,
    duration: '6 Months'
})
```
- Inserts multiple documents into a MongoDB collection in a single operation.
```
insertMany
```
```
db.courses.insertMany([
    {
    title: 'C++',
    description: 'C++ Programming with OOP's',
    fees: 499,
    duration: '3 Months'
    },
    {
    title: 'Data structures',
    description: 'Data Structures and Algorithms',
    fees: 999,
    duration: '6 Months'
    },
])
```
![screenshot](./Output/insertMany.png)

- Queries a collection to retrieve documents based on specified criteria. It can be used to search for multiple documents.

``` 
find()
1. db.students.find()

findOne()
```
![screenshot](./Output/find.png)

- Removes a single document from a collection that matches a specified filter.

```
deleteOne()
 db.courses.deleteOne({_id: ObjectId("652f7387434758e91eb89af4")})

deleteMany()
```
![screenshot](./Output/deleteOne.png)

- Modifies the first document that matches a specified filter in a collection, making the specified updates.

```
updateOne()
```
![screenshot](./Output/updateOne.png)

- Updates multiple documents in a collection that match a specified filter with the specified changes.

```
updateMany()
```
![screenshot](./Output/updateMany.png)


