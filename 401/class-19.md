# Read 18: AWS: API, Dynamo and Lambda (in progress)

1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server - 
   They are both able to receive, process and respond to HTTP requests. Labmda functions are same as handler functions in ExpressJS Server in that they get triggered(invoked) when a certain endpoint gets hit with an appropriate request.

2. List the AWS Database offerings and talk about the pros and cons of each
   ([Ref](https://skelia.com/articles/aws-database-services/))
   * **Relational Databases**
     - Amazon Aurora
     - Amazon RDS
     - Amazon Redshift

- Benefits of relational databases
  - They use SQL (Structured Query Language), which is quite widespread and supports join operations by default.
  - The simple structure allows you to effectively work with most data types.
  - You have the ability to quickly update data. The entire database is stored on one computer, and the relationships between the records are used as pointers, that is, you can update one record and all records associated with it will be immediately updated.
  - Relational databases support atomic transactions.
  - Relational databases offer high security. You can limit or allow data access for specific users. 
- Disadvantages of relational databases
  - Scaling is done by adding computing power to the computer on which the database is installed. This method is called vertical scaling. However, why is this a disadvantage? Because there is a limit to the computing power of a computer and adding resources encourages downtime.
  - OOP objects are not supported, so even representing simple lists can be a problem.
  - Since each query is against the entire table, the execution time of the query depends on the size of the table. This is an important limitation that forces us to keep tables relatively small and optimize the database to scale.
  - The relational data approach is not suitable for all domains.
   
   * **NoSQL Databases**
     - Document DB
     - Dynamo DB
     - Neptune
     - QLDB

- Advantages of NoSQL database
  - They allow you to store objects of various structures.
  - They can display almost all data structures, including OOP objects, lists and dictionaries, using good old JSON.
  - NoSQL queries are super fast. Each record is independent and therefore the query time is independent of the size of the database.
  - Although the nature of NoSQL isn’t schematic, they often support schema validation. This means that you can make a collection with a schema. This schema will not be as simple as a table. It will be a JSON schema with specific fields.
  - You can make the most out of the AWS Cloud database, delivering zero downtime.
  - In NoSQL, database scaling is carried out by adding computers and distributing data between them. It allows you to automatically add resources to the database when you need them, without causing downtime.
- Disadvantages of NoSQL database
  - Updating data is a slow process in a document database because data can be shared between computers and can be duplicated.
  - Atomic transactions are not supported by default. 
  - There is strong attachment of the application to a specific DBMS due to the specifics of the internal query language and a flexible data model focused on a specific case.
   
3. What’s the difference between a FIFO and a standard queue? - 

FIFO - strict order of queue delivery is preserved, standard queue - not preserved.

4. How can the server be assured a message was properly received? -  

By triggering an event within the receiver that listens to a message. Server then can listen to an event itself from a receiver that will send out an event once a message is received.

## Vocabulary

- Serverless API - does not require a developer to worry about an infrastructure when building an API.
  
- Triggers - Any event that a functions is listening for. 
  
- Dynamo vs Mongo 
  ([Source](https://www.bmc.com/blogs/mongodb-vs-dynamodb/))
  - MongoDB is platform-agnostic. DynamoDB is limited to AWS.
  - DynamoDB is a fully managed database that allows users to start using the database straightaway, as AWS will manage all the scaling, availability, and updates. It enables provisioning a multi-region, highly available database with just a few clicks, drastically reducing the need for dedicated infrastructure management.
  On the other hand, MongoDB requires users to manage all the infrastructure and configurations for a based MongoDB deployment. Though this provides users with the greatest degree of control over the database, it comes with increased complexity.
  - MongoDB is a schema-free database. Schemas can be enforced. DynamoDB is a schema-less database but with no ability to enforce schemas.

- Dynamoose vs Mongoose
  - Dynamoose is an ORM for AWS DynamoDB
  - Mongoose is an OM for MongoDB

## Preparation Materials

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)
[AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

## Bookmark

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)
[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)

[**<== BACK**](401-toc.md)

