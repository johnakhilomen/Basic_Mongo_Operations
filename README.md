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
# Get data from collection
```python
db.movies.find();
```

# Drop collection:
```python
db.movies.drop()
```
