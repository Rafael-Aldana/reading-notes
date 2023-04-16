# AWS: Events

## AWS SQS vs SNS

What is the difference betweeen SQS and SNS?

SNS is typically used for applications that need realtime notifications, while SQS is more suited for message processing use cases. SNS does not persist messages - it delivers them to subscribers that are present, and then deletes them. In comparison, SQS can persist messages (from 1 minute to 14 days).

What are some use cases for both SNS and SQS?

Using SNS and SQS together, messages can be delivered to applications that require immediate notification of an event, and also persisted in an SQS queue for other applications to process at a later time. You can also combine SNS and SQS to ensure end-to-end message ordering.

## AWS SNS and SQS

Describe how to use SQS and SNS in a “fanout” pattern.

In a "fanout" pattern, messages are sent from a single source to multiple destinations, where each destination receives a copy of the same message.

To achieve this pattern using SQS and SNS, we can set up an SNS topic to act as a central hub for incoming messages. Subscribed to this topic can be one or more SQS queues, which receive copies of the messages.

When a message is sent to the SNS topic, it will be forwarded to all of the subscribed SQS queues, which can then process the message independently. This allows us to decouple the sending and receiving components of our application, and to scale the number of receivers horizontally as needed.

In addition, by using SQS and SNS together, we can ensure that messages are reliably delivered to all subscribers, even if one or more of the receivers is temporarily unavailable.

Explain how “push notifications” work, using SNS.

Push notifications are messages that are "pushed" to a user's device, such as a smartphone or tablet, even when they are not actively using an app. In Amazon Web Services, Simple Notification Service (SNS) is a fully managed messaging service that enables you to send notifications to different types of endpoints.

When you want to send a push notification to a user's device, you can use SNS to publish a message to a specific topic. The topic is essentially a channel or category that subscribers can receive notifications from.

In order to receive the notification, the user's device must be subscribed to the topic. This is typically done by the user through the app settings or preferences. When the user subscribes to the topic, they provide the device token, which is a unique identifier for the device.

Once the message is published to the topic, SNS uses the device token to send the message directly to the user's device via the appropriate push notification service (such as Firebase Cloud Messaging or Apple Push Notification Service). The message is then displayed as a notification on the user's device, even if the app is not currently open.

## SQS and SNS Basics

How might a large scale, distributed application make use of a Queue system like SQS?
 let's say we have an e-commerce application that processes orders from customers. When a customer places an order, the order data is sent to an API endpoint, which then sends the order to a processing service that validates the order and updates the inventory. However, during peak periods, such as holidays, the processing service might become overloaded, causing requests to time out or fail. To avoid this situation, we can use a queue system like SQS to offload the processing work from the API endpoint to the processing service. The API endpoint can simply send the order data to an SQS queue, and the processing service can then poll the queue to retrieve and process orders at a rate it can handle, without being overwhelmed by spikes in traffic.

In this scenario, SQS provides several benefits:

Decoupling: The API endpoint and processing service are decoupled, meaning they don't have to communicate directly with each other. This enables us to scale them independently and avoid cascading failures if one of them goes down.
Resilience: SQS is a highly available service that automatically replicates messages across multiple availability zones, making it resilient to failures.
Elasticity: SQS is highly scalable and can handle millions of messages per second, enabling us to handle spikes in traffic and adjust capacity dynamically.
Asynchronous processing: Using SQS enables us to process messages asynchronously, which can improve the overall performance and reliability of our application.

[link-to-reading-notes](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5).
[link-to-reading-notes](https://www.youtube.com/watch?v=mXk0MNjlO7A).
[link-to-reading-notes](https://www.youtube.com/watch?v=UesxWuZMZqI).

## Bookmark and Review

[link-to-reading-notes](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html).
[link-to-reading-notes](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?