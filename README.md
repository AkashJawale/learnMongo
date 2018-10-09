# learnMongo

# for create database
 - use <database name>
 Ex-> use Akash
 
# know in which database you work
 - db
# show database 
 -> show dbs
 
# drop database
- db.dropDatabase()

# Create collection
- db.createCollection ("Database name")
Ex-> db.createCollection("Akash")

# show collection
 - show collections
 
 
 # How to add data in document
 - db.employee.insert ( {
   name:'akash'
  })
  
  
# Find data
Ex->  db.employee.find ({"Gender" : "male"})


# show data from Database
 - db.employee.find ({})

# less than equal condition
db.Akash.find ({"Age":{$lt:"30"}})
[$lt means less than
$lte means less than or equal to
$gte means greater than or equal to
]

# include two conditions
db.employee.find({$or :[
{"Age" : {$gt:"30"}},
{"Gender" :"male"}
]})
