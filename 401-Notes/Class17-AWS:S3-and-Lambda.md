# AWS: S3 and Lambda

## AWS S3

What is Amazon S3?

Amazon S3 or Amazon Simple Storage Service is a service offered by Amazon Web Services that provides object storage through a web service interface. Amazon S3 uses the same scalable storage infrastructure that Amazon.com uses to run its e-commerce network.

Name some use cases for Amazon S3.

Amazon S3 (Simple Storage Service) is a cloud-based object storage service offered by Amazon Web Services (AWS). Here are some common use cases for Amazon S3:

File storage: Amazon S3 can be used to store and retrieve any amount of data at any time, making it an ideal solution for file storage.

Backup and disaster recovery: Amazon S3 provides a reliable, scalable, and cost-effective solution for backup and disaster recovery. You can use S3 to store backups of your critical data and applications, and recover them quickly in case of any disaster.

Media storage and distribution: Amazon S3 can be used to store and distribute media files such as videos, music, and images. It is designed to deliver high-speed content and low-latency performance.

Data archiving: Amazon S3 provides long-term data archiving capabilities, allowing you to store data for years at a low cost.

Big data analytics: Amazon S3 can be used as a data lake to store large amounts of unstructured data for big data analytics.

Static website hosting: Amazon S3 can be used to host static websites, providing a simple and cost-effective way to host a website.

Cloud-native application development: Amazon S3 provides APIs for developers to build cloud-native applications that can scale quickly and handle large amounts of data.

Name some benefits of using Amazon S3.

Scalability: Amazon S3 can handle any amount of data and can scale to meet the needs of any application.

Durability: Amazon S3 is designed to provide 99.999999999% durability, meaning that your data is highly resistant to loss or corruption.

Security: Amazon S3 provides a number of security features, including encryption at rest and in transit, access control, and audit logs.

Cost-effective: Amazon S3 pricing is based on usage, so you only pay for what you use.

Easy to use: Amazon S3 is easy to set up and use, with a simple web interface and APIs for easy integration with other applications.

Integration with other AWS services: Amazon S3 integrates with other AWS services, such as EC2, Elastic Beanstalk, and Lambda, allowing you to build highly scalable and efficient applications.

## AWS Lambda Basics

What is AWS Lambda?

AWS Lambda is an event-driven, serverless computing platform provided by Amazon as a part of Amazon Web Services. It is a computing service that runs code in response to events and automatically manages the computing resources required by that code.

Name some use cases for AWS Lambdas.

AWS Lambda is a serverless computing platform that allows developers to run code without managing servers. Some use cases for AWS Lambda include:

Event-driven computing: AWS Lambda can be used to trigger code automatically in response to events from other AWS services, such as S3, DynamoDB, or API Gateway. This makes it a great fit for event-driven applications and serverless architectures.

Backend processing: Lambda functions can be used to process data, such as image or video transcoding, data validation, and data transformation. This can offload the processing from the main application, making it more efficient and scalable.

Real-time stream processing: AWS Lambda can be used to process real-time streams of data, such as logs, clickstreams, or social media feeds. This can allow developers to quickly process and analyze data as it is generated.

Chatbots: AWS Lambda can be used to build chatbots that can respond to user input and perform actions. For example, a chatbot could be built to handle customer service inquiries, order processing, or appointment scheduling.

Webhooks: Lambda functions can be used to process data sent from external services via webhooks. This can be useful for integrating with third-party APIs, such as payment gateways or marketing platforms.

Scheduled tasks: AWS Lambda can be used to run scheduled tasks, such as backups, data archiving, or data processing. This can help automate routine tasks and reduce manual intervention.

Describe “serverless” to a non-technical friend.

"Serverless" is a term used to describe a way of building and running applications where you don't have to worry about managing servers or infrastructure. Instead of worrying about setting up and managing servers, you can focus on writing the code for your application. The cloud provider (such as AWS) will handle all the underlying infrastructure for you, automatically scaling it up or down as needed. This means you only pay for what you use, and you can deploy and update your application quickly and easily. It's like renting a car instead of buying one - you can use it when you need it and return it when you're done, without having to worry about the upkeep and maintenance.

## CDN

What is a CDN?

Amazon CloudFront is a content delivery network operated by Amazon Web Services. Content delivery networks provide a globally-distributed network of proxy servers to cache content, such as web videos or other bulky media, more locally to consumers, to improve access speed for downloading the content.

How does a CDN work with relation to the website visitor?

A CDN, or Content Delivery Network, works by placing a network of servers around the world in strategic locations. When a website visitor requests to view a website hosted on a server, the CDN will automatically determine the visitor's geographic location and will serve the website content from the server closest to that visitor, rather than from the website's original server. This results in faster load times and a better user experience for the visitor. Additionally, the CDN can also cache frequently accessed content, which further reduces load times and can help to handle large traffic spikes without affecting the performance of the website.

What are the benefits of employing a CDN?

Faster content delivery: By caching content on servers located closer to the end user, a CDN can deliver content faster and more reliably, reducing load times and improving the overall user experience.

Scalability: A CDN can handle sudden spikes in traffic by distributing the load across multiple servers, reducing the risk of downtime or slow performance.

Lower server costs: By offloading static content to a CDN, web servers can focus on processing dynamic content, reducing the overall server load and potentially lowering costs.

Improved SEO: Faster load times and better availability can improve search engine rankings, helping to attract more visitors to a website.

Global reach: A CDN can distribute content to servers around the world, allowing businesses to reach a wider audience and improve their global presence.


[link-to-reading-notes](https://aws.amazon.com/s3/).
[link-to-reading-notes](https://www.serverless.com/aws-lambda).
[link-to-reading-notes](https://cyberhoot.com/cybrary/content-delivery-network-cdn/).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?