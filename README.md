# json_data
JSON data

***Create Database***
```python
use moviedb
```

# import json data
```python
mongoimport --db moviedb --collection movies --file /Users/user1/Downloads/json_data-main/movies.json
mongoimport --db moviedb --collection users --file /Users/user1/Downloads/json_data-main/users.json
```
# Get all
```python
db.movies.find();
```

# Get one
```python
db.users.findOne({Username: "jondoe2"});
```

# Drop collection:
```python
db.movies.drop()
```

# Update collection
```python
db.users.update({Username: "jondoe2"}, {$set: {Email: "newjondoe2@email.comdb.users.update({Username: "jondoe2"}, {$set: {Email: "newjondoe2@email.com", Password: "newpasscode1"} } )
```

# Delete one
```python
db.users.remove({Username: "jondoe2"});
```

# Get sub object
```python
db.movies.find({"Genre.Name": "Thriller"})
```
## Mongo import for remote db
```python
mongoimport --uri mongodb+srv://readnwriteuser:your_password@cluster0.plvbm.mongodb.net/myFirstDatabase --collection movies --file /Users/johnakhilomen/Downloads/json_data-main/movies.json --type json
```
