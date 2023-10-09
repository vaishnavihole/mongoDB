## MongoDB commands for Databases


### View all databases
> show dbs

### Create a new or switch databse
> use dbName

### View current databases
> db

### Delete databases
> db.dropDatabase()

## MongoDB commands for Collections

### Show Collections
> show collections

### Create a collection 
>  db.createCollection **(collection name)**

### Delete Collection
> db.**collectionName**. drop()

### MongoDB commands for Rows

### Insert One Rows:-
>db. **collectionName** .insert({})

***Example***
```js
db.student.insert({
    'name': 'ABC',
    'lang': 'English',

})
```

### Insert  Many Rows:-
>db. **collectionName** .insertMany ( [ { } ] )

***Example***
```js
db.students.insertMany([{
    'name': 'ABC',
    'lang': 'JavaScript',
     }, 
    
    {'name': 'XYZ',
    'lang': 'HTML',
     }, 
     4
     {'name': 'PQR',
     'lang': 'DSA',
     }
     ])
```
### Show all Rows in Collection:-
>db. **collectionName**.find()

 ## Find the first row matching the object:-
 >db.**collection name**.findOne({key: 'value'})


### Show all Rows in Collection (     Prettified):-
>db. **collectionName**.find().preety()

## Search in MongoDB Database:-
> db.collectionName.find({key: 'value'})

***Example***

> db.students.find(`{lang: 'DSA'}`)

## Limit the number of rows in output:-
>db.collectionName.find().limit(number)

## Count the number of rows in the output:-
>db.collectionName.find().count()

 ## Update a document:-
>db.collectionName.update({key: 'value'}, {$set: {key: 'updated value'}}) 

## MongoDB Increment Operator:-

```js
db.comments.update({key: 'value'},
{$inc:{
    key : 'value'
}})
```

## MongoDB Rename Operator:-

```js
db.comments.update({key: 'value'},
{$rename:{
    key : 'value'
}})
```

## Delete Row:-
```js
db.comments.remove({key: 'value'})
```

