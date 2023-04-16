# AWS: API, Dynamo and Lambda

## AWS API Gateway Overview

What is Amazon API Gateway?

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.

Why is Amazon API Gateway an important part of the Serverless ecosystem?

Amazon API Gateway is an important part of the Serverless ecosystem because it acts as a front door for your serverless applications. When you build a serverless application, you need a way to expose your application to the internet, and API Gateway provides a scalable and secure way to do this.

API Gateway makes it easy to create, publish, and manage APIs for your serverless applications. It allows you to define HTTP endpoints that can trigger Lambda functions, and it can also be used to integrate with other AWS services like S3, DynamoDB, and more. Additionally, API Gateway provides features like rate limiting, caching, and authentication to help you build robust and secure APIs.

By using API Gateway, you can focus on building your application logic without worrying about the infrastructure and scaling issues. API Gateway takes care of the scaling and availability of your APIs, and it can handle large amounts of traffic with ease. This makes it a critical component of the Serverless ecosystem, allowing developers to build and deploy serverless applications with confidence.

How does API Gateway integrate with other AWS services?

You can integrate many AWS services with API Gateway, but the setup and mapping vary depending on the particular service API. To integrate another service with API Gateway, build an HTTPS request from API Gateway to the service API so that all request parameters are correctly mapped.

## AWS API Gateway

What are the some benefits of using Amazon API Gateway?

Scalability: Amazon API Gateway can handle millions of API requests and automatically scales to meet traffic demands.

Easy Integration: Amazon API Gateway makes it easy to integrate with other AWS services such as AWS Lambda, Amazon S3, and Amazon DynamoDB.

Security: Amazon API Gateway provides security features such as authentication, authorization, and SSL/TLS encryption to protect APIs from unauthorized access.

Monitoring and Analytics: Amazon API Gateway provides real-time monitoring and analytics to help developers troubleshoot issues and optimize performance.

Cost-effective: Amazon API Gateway offers a pay-as-you-go pricing model, which means developers only pay for the API calls they receive and the amount of data transferred.

Flexibility: Amazon API Gateway supports a wide range of API protocols and allows developers to customize their API behavior using AWS Lambda functions, HTTP responses, and other features.

What two API types might you choose from?

There are two main types of APIs that you can choose from when designing an API with Amazon API Gateway: REST APIs and WebSocket APIs.

REST (Representational State Transfer) APIs are designed to expose resources and allow you to perform operations on them using standard HTTP methods such as GET, POST, PUT, and DELETE. REST APIs are typically used for building HTTP-based web services that are accessible from a variety of client applications.

WebSocket APIs, on the other hand, are designed to allow real-time communication between a client and server over a persistent, bidirectional connection. WebSocket APIs are ideal for building chat applications, real-time gaming applications, and other applications that require low latency and real-time data transfer.

## AWS DynamoDB Guide

What is DynamoDB?

Amazon DynamoDB is a fully managed proprietary NoSQL database service that supports key–value and document data structures and is offered by Amazon.com as part of the Amazon Web Services portfolio. DynamoDB uses synchronous replication across multiple data centers for high durability and availability.

Under what circumstances would you recommend DynamoDB over MongoDB?

Scalability: DynamoDB is highly scalable and can handle massive workloads with ease. This makes it a good choice for applications with unpredictable or rapidly changing traffic patterns.

Availability: DynamoDB is designed for high availability, with built-in features like multi-AZ deployments and automatic failover. This makes it a good choice for applications that need to be highly available.

Performance: DynamoDB is optimized for fast reads and writes, and can handle large volumes of data with low latency. This makes it a good choice for applications that require high performance.

Serverless: DynamoDB integrates well with AWS serverless services like Lambda and API Gateway, allowing you to build fully serverless applications that can scale quickly and efficiently.

## AWS DynamoDB

Explain to a non-technical friend how DynamoDB works.

In DynamoDB, you can store data in tables. Each table has a primary key that uniquely identifies each item in the table. When you add an item to a table, it's automatically indexed by the primary key for fast and efficient retrieval.

One of the key features of DynamoDB is that it is fully managed by AWS. This means that AWS takes care of things like scaling and maintenance for you, so you don't have to worry about managing the infrastructure yourself.

DynamoDB is also designed to be highly available and durable. It automatically replicates your data across multiple availability zones within a region, so if one zone goes down, your data is still available from another zone.

Overall, DynamoDB is a powerful and flexible database service that can be used for a wide range of applications, from small-scale projects to large-scale enterprise systems.

## Dynamoose

What is Dynamoose?

Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familiar.

What are some key features of Dynamoose?

Schema Definition: Dynamoose allows you to define a schema for your data, which helps ensure consistency and reduces errors. You can define properties, data types, default values, and validation rules for your data.

Middleware: Dynamoose supports middleware, which allows you to add custom behavior to your data models at various stages of the lifecycle, such as before or after saving or deleting data.

Querying: Dynamoose supports a wide range of query types, including basic CRUD operations, complex queries with multiple conditions and filters, and batch operations.

Type Checking: Dynamoose supports type checking, which helps ensure that your data conforms to the defined schema.

Promise-based: Dynamoose is promise-based, which makes it easy to use with modern JavaScript frameworks and libraries that support asynchronous programming.

[link-to-reading-notes](https://www.serverless.com/amazon-api-gateway).
[link-to-reading-notes](https://aws.amazon.com/api-gateway/).
[link-to-reading-notes](https://www.dynamodbguide.com/what-is-dynamo-db/).
[link-to-reading-notes](https://aws.amazon.com/dynamodb/).
[link-to-reading-notes](https://dynamoosejs.com/getting_started/Introduction).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?