# express-test
Playing around with Express, MongoDB and Jade

## Getting started

Make sure you have [Node](https://nodejs.org/en/) and [MongoDB](https://docs.mongodb.org/manual/installation/) installed.

If you have brew installed you can use:
```
brew update
```
```
brew install mongodb
```

Then `cd` into your project folder and run:
```
npm install
```
When that is done, create a data folder for the database
```
mkdir data
```

Then in a terminal window attach MongoDB to your data folder
```
mongod --dbpath [path/to/your/data/folder]
```

Then we need to get into MongoDB's CLI
```
mongo
```

Then tell is too use your project
```
use [project-name]
```

Then we can add in some test data, just to make sure it ios working when we bott up
```
db.userlist.insert({'username' : 'test1','email' : 'test1@test.com','fullname' : 'Bob Smith','age' : 27,'location' : 'San Francisco','gender' : 'Male'})
```

Finally run
```
npm start
```

##Contents

* /public - static directories suchs as /images
* /routes - route files for project
* /views - views for project
* README.md - this file
* app.js - central app file for project
* package.json - package info for project