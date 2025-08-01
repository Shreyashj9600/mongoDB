### 📘 Basic MongoDB Commands Cheat Sheet (CMD / mongosh)


# 🔹 Start MongoDB Shell
mongosh

# 🔹 Show all databases
show dbs

# 🔹 Switch to / Create a new database
use myDatabase

# 🔹 Show current database
db

# 🔹 Show all collections in current DB
show collections

# 🔹 Insert one document
```
db.users.insertOne({ name: "Shreyash", age: 21 })
```

# 🔹 Insert multiple documents
```
db.users.insertMany([
  { name: "Amit", age: 22 },
  { name: "Ravi", age: 20 }
])
```

# 🔹 Find all documents in a collection
```
db.users.find()
```

# 🔹 Find with a condition
```
db.users.find({ age: 21 })
```

# 🔹 Update one document
```
db.users.updateOne(
  { name: "Shreyash" },
  { $set: { age: 22 } }
)
```

# 🔹 Delete one document
```
db.users.deleteOne({ name: "Amit" })
```

# 🔹 Drop a collection (delete it)
```
db.users.drop()
```

# 🔹 Drop the current database
```
db.dropDatabase()