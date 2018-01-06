# Getting started with Mongodb on Windows

*This guide covers the setup to run Mongodb 3.6 on Windows 10 with default settings*

1. Download and run [Mongodb CE](https://www.mongodb.com/download-center#community)

2. Add `C:\Program Files\MongoDB\Server\3.6\bin` to PATH; so that `mongod`, `mongo` can run on any directory

3. `mkdir data\db` ; Create default data folder in C:\ for mongodb

4. Run `mongod` to run the Mongo server on port 27017

5. Run `mongo` on another terminal window to run shell to perform queries on database.

## Run simple commands

To test the config is working:

+ Running `db` on `mongo` terminal should return `test`

INSERT:

+ `db.data.insert({"username": "tom"})`

FIND:

+ `db.data.find()`
