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


> Note: A collection is automatically created whenever we create/insert a document in it.
Ex: 
![Screenshot 2023-11-30 181915](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/fe1fe26d-fc8a-40dc-9aa9-ab872b03b5d7)

* Here we are not creating any collection(data is the automatically created collection in this case) before inserting the document.


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


* **Inserting a document to the collection named 'data'**

```mongodb
students> db.data.insertOne({'name': 'Vivek', age: 24})
```
![Screenshot 2023-11-30 183716](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/25d9f867-4cb9-4ca5-bcbe-d0aa8725292b)


* **Inserting many documents to the collection named 'data'**

```mongodb
students> db.data.insertMany([{'name': 'Vivek', age: 24}, {'name': 'Pratap', age: 20},{'name': 'Ranjeet', age: 25}])
```
![Screenshot 2023-11-30 185204](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/cccf5b44-5859-40f6-b783-8744695fb25c)


#### Command to list all documents.
***
```bash

students> db.data.find()
```

Example.
![Screenshot 2023-12-01 203818](https://github.com/codingXpert/express_sequelize_mysql_crud_api/assets/101451924/99500dcf-6930-46f6-a253-83d70045d302)


#### When to use quotes and when not to.
***
![Screenshot 2023-12-01 210729](https://github.com/codingXpert/express_sequelize_mysql_crud_api/assets/101451924/827abc62-fe78-43a5-bd72-b7b25aac039a)

![Screenshot 2023-12-01 211705](https://github.com/codingXpert/express_sequelize_mysql_crud_api/assets/101451924/9c2f404e-ceec-4013-a155-f2c6100010db)


#### Ordered and Unordered Insert.
***
![Screenshot 2023-12-04 091032](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/7226ac19-90d0-44bd-978b-910bcef603a3)

**Examples**
![Screenshot 2023-12-04 091526](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/1140bde8-02a2-48df-8263-1b5ca26b6a1b)

![Screenshot 2023-12-04 091543](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/d68a9e8f-49f8-4cd9-bcaa-6a7906c4ed9f)


#### Case Sensitivity.
***
![Screenshot 2023-12-04 103435](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/195796b3-fc52-403e-9b2c-0b44a955ea2b)


#### Finding documents in mongoDB.
***
![Screenshot 2023-12-04 103949](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/44183d9c-2656-4c5e-bf2a-0983812625c2)

**Examples**
![Screenshot 2023-12-04 104151](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/2582f5f1-e667-4f16-a56b-3371c64c057e)

![Screenshot 2023-12-04 104151](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/8d21abf7-6247-4af1-8408-bc4b5aeae179)


#### Importing JSON in mongoDB.
***
> When the JSON is not inside an Array(single document).
![Screenshot 2023-12-04 104641](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/16fa8942-b45d-4a6c-b995-b66bb490cf44)

> When the JSON is inside an Array(multiple documents).
![Screenshot 2023-12-04 104658](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/d81aa0fd-4be6-41d1-9a1c-c540326bf9d7)

> Example.
![Screenshot 2023-12-04 124336](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/6704e348-3e97-4652-b8c3-4b8fc3b9436c)


#### Importing And Exporting JSON in mongoDB.
***
![Screenshot 2023-12-04 122702](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/b3a829c7-d466-4ccd-a5f3-d4e21b044a7e)

![Screenshot 2023-12-04 123056](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/974231d4-d189-490e-9585-1162ca24b88d)


#### Comparison Operator.
***
![Screenshot 2023-12-04 125043](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/9240929d-818b-4ab3-b459-390ab58895c4)

![Screenshot 2023-12-04 125315](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/739ad57a-09fb-4122-b3da-a7e9278c4704)

> Note.
* **eq:-** Equals To.
* **ne:-** Not Equals To.
* **gt:-** Grater Than.
* **gte:-** Grater Than Equals To.
* **lt:-** Less Than.
* **lte:-** Less Than Equals To.
* **eq:-** In Operator(Compares with multiple data).
* **eq:-** Not In Operator.
 

#### Introduction To Cursors.
***
![Screenshot 2023-12-04 135622](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/1760ea5a-ad30-48e0-9baf-03a1e0640e44)

#### Available Cursors Methods.
![Screenshot 2023-12-04 135737](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/47d748ce-e3e6-4587-9a58-37709e565890)

**Examples**
![Screenshot 2023-12-04 140902](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/52e607b0-7ad5-41f1-a22f-2afaa646eb61)

![Screenshot 2023-12-04 141016](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/94d049d4-ab2b-4ad7-b90b-716be06d806c)


#### Caution while using Cursors.
***
![Screenshot 2023-12-04 141506](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/626e5aa0-bd0f-4885-9cc8-8e60f9bc35eb)


#### Logical Operator.
***
![Screenshot 2023-12-04 144017](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/fac9ba30-1ca1-4514-9889-448fa6140b11)

> **Logical AND**.
![Screenshot 2023-12-04 144138](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/55b4920f-807b-4dfc-90b3-429d1e48c039)

**Example**
![Screenshot 2023-12-04 144512](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/747d9177-5227-40ed-9107-a92d8d31cc5a)

> **What if we don't use AND Operator**
![Screenshot 2023-12-04 144622](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/ab16d121-b01c-4f3c-9481-779c97719fb1)

**Example**
![Screenshot 2023-12-04 144555](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/64dbe248-f978-415b-82fa-88bc68e4a2ef)


> **Logical OR**.
![Screenshot 2023-12-04 145541](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/c06f94d0-ef40-4d4d-a038-8bc3644a97bf)

**Example**
![Screenshot 2023-12-04 145630](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/8b9f9ddc-0598-4f9e-b641-3ace03a16baa)


> **Logical NOR(Opposite of OR)**.
![Screenshot 2023-12-04 150113](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/b38e471d-7c7e-4ad5-996c-6316b725c15f)

**Example**
![Screenshot 2023-12-04 145952](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/d46adf04-458b-4066-ae1f-2cb3b225b600)


> **Logical NOT**.
![Screenshot 2023-12-04 150612](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/2fc86e0e-2762-4a44-bb7a-037998d49c4f)

**Example**
![Screenshot 2023-12-04 150542](https://github.com/codingXpert/Mongo-DB-Notes/assets/101451924/0d05a5e4-5c1e-4f86-8dc1-48ed4081fcf7)




