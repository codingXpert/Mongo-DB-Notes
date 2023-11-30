![Screenshot 2023-11-29 175201](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/c4b6357b-994e-4533-b8a1-badfa6c2e742)

![Screenshot 2023-11-29 175208](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/9ff1a423-bbac-47a6-88f7-ce14b8e63f4e)

![Screenshot 2023-11-29 175332](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/1168565b-2d24-430b-a53a-e7d13adcfa98)

![Screenshot 2023-11-29 175511](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/5e43045f-288e-41eb-b522-dfb65a0a5f2f)

![Screenshot 2023-11-29 121007](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/7ceb68c5-81d3-4719-b85f-98b49f2f8c7f)

![Screenshot 2023-11-29 175926](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/fb29eb56-5cc3-4d2c-92cc-3f71f467ef18)

![Screenshot 2023-11-29 180114](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/8cdcd323-74a1-43b1-bb0e-29909066caad)

![Screenshot 2023-11-29 180211](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/33d30bee-97f5-4ac2-b8c0-80250ec3d241)

![Screenshot 2023-11-29 180502](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/df8b5510-41c9-47bc-b2c7-273d22ae7d18)

![Screenshot 2023-11-29 182013](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/b87ce9f7-50f2-4817-b6e7-68b3b169b335)

![Screenshot 2023-11-29 182025](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/2973dbf6-09e5-4209-8660-1797a0dcc986)

![Screenshot 2023-11-29 182314](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/8a6a5af1-1949-4db2-b23c-ef12a96cbc63)

![Screenshot 2023-11-30 150655](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/af6b681c-64e9-40f6-8c66-65b4663788c0)

![Screenshot 2023-11-30 150815](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/82a7deb6-8e31-478c-959b-e54f7bc819b5)

![Screenshot 2023-11-30 150916](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/aa7ba21b-6c05-4965-8aec-b382db0d723e)

![Screenshot 2023-11-30 160329](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/0db93995-b8a5-4584-a701-b3bfc9aa4a8a)


### Working with mongoDB Shell.
***

* Install the mongodb shell from [Here](https://www.mongodb.com/try/download/shell).
* After Installation Open the terminal and type mongosh to start mongodb shell.
* we can also start the mongodb shell directly from the installed file by double clicking it and providing it the host(mongodb://localhost:27017), Like this:- 

![Screenshot 2023-11-30 162323](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/234fac34-ec82-4fb9-bc95-454a46720db8)

* After successful connection we will get a screen like this(where we can write our db commands):-

![Screenshot 2023-11-30 162349](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/dcfc0bde-cc61-42fb-ba83-d062708123fd)

#### Command to list all the available Databases.
***
```bash

 show dbs Or show databases(not db or database)
```

![Screenshot 2023-11-30 162954](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/4a2bdc81-39dc-4efc-a975-452f90b568f2)


#### Command to clear the screen.
***
```bash

 cls
```

#### Command to use any existing db(or creating as well as using it).
***
```bash

 use <database name>

 ex: use students
```

* Example

![Screenshot 2023-11-30 173148](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/b0dbd72c-c21d-4ee9-83a5-bc0668d762e2)

* In the above example we are inside the students db , but when we are listing the dbs there is no db name students. This is because of👇.
![Screenshot 2023-11-30 160901](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/e9f40d42-0704-4d62-8a75-b9784eb8e037)

* Creating a collection in students db.

```bash
db.createCollection('collectionName')

ex:
db.createCollection('data')
```

![Screenshot 2023-11-30 174353](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/7c2a96e0-e260-4be6-8ec8-e15f691e3258)

* Now listing the dbs again and this time the **students db** will be listed.
![Screenshot 2023-11-30 174421](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/356aefe9-51cb-4f2e-8818-2fbea62ba7b3)


#### Command to list all collections.
***
```bash
show collections
```

#### Command to delete/drop a collection.
***
```bash
db.collectionName.drop()

ex: db.data.drop()
```
![Screenshot 2023-11-30 180333](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/15a77bb4-8a34-4a54-b494-a0441c81f296)


#### Command to delete/drop a database.
***
```bash
db.dropDatabase()

ex: db.dropDatabase()
```
![Screenshot 2023-11-30 180716](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/1bb03e0c-87b4-410c-8ea5-f1ef0e95bb4e)


### insertOne and insertMany (data) in the db collection as document.
***
![Screenshot 2023-11-30 181007](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/278c3076-2dc1-46c7-b42d-8d65b4168a94)

![Screenshot 2023-11-30 181121](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/cf1366e9-0ef2-4d3a-91df-59c3fc9b75d3)

![Screenshot 2023-11-30 181140](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/1639a3c2-4a7e-4038-bee5-526baa918be3)
