### Insert
db.collection.insertOne()
> db.people.insertOne({ firstName: "first", lastName: "last"})

db.collection.insertMany()
> db.people.insertMany({ firstName: "first", lastName: "last"}, { firstName: "one", lastName: "two"})

### Update
db.collection.updateOne(<filter>, <update>, <options>)
> db.people.updateOne(
    { firstName: "one"},
    {
        $set: { "lastName": "second" }
    }
)

db.collection.updateMany(<filter>, <update>, <options>)
> db.people.updateMany(
    { age: { $lt: 10} },
    {
        $set: { "lastName": "second" }
    }
)

### Delete
db.collection.deleteMany()
> db.people.deleteMany({ city: "Palembang" })

db.collection.deleteOne()
> db.people.deleteOne({ id: 1 })