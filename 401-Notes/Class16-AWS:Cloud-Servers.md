# AWS: Cloud Servers

## AWS EC2

What is an EC2 Instance?

An Amazon EC2 instance is a virtual server in Amazon's Elastic Compute Cloud (EC2) for running applications on the Amazon Web Services (AWS) infrastructure.

Name 2 use cases for EC2.

Run cloud-native and enterprise applications - Amazon EC2 delivers secure, reliable, high-performance, and cost-effective compute infrastructure to meet demanding business needs.

Scale for HPC applications - Access the on-demand infrastructure and capacity you need to run HPC applications faster and cost-effectively.

Develop for Apple platforms - Build, test, and sign on-demand macOS workloads. Access environments in minutes, dynamically scale capacity as needed, and benefit from AWS’s pay-as-you-go pricing.

Train and deploy ML applications - Amazon EC2 delivers the broadest choice of compute, networking (up to 400 Gbps), and storage services purpose-built to optimize price performance for ML projects.

Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

One of the main advantages of ECS over these other services is that it is fully customizable and can be integrated with other AWS services. For example, you can use ECS to deploy applications to an EC2 instance or a cluster of EC2 instances, or you can use it to deploy containers to AWS Fargate, a serverless compute engine for containers. ECS also allows you to configure load balancing, auto scaling, and service discovery, which can be very useful for larger and more complex applications.

In addition, ECS provides a high level of security and compliance with various industry standards, such as HIPAA and PCI DSS. This can be especially important for companies in regulated industries, such as healthcare or finance.

Overall, while Heroku, Digital Ocean, Render.com, and other similar services may be more convenient for smaller and less complex applications, ECS is a better choice for larger and more complex applications that require a high level of flexibility, control, and security.

## EC2 For Humans

Where can we find EC2 on the AWS Console?

You can find EC2 (Elastic Compute Cloud) on the AWS (Amazon Web Services) console by following these steps:
Log in to your AWS account.
Go to the AWS Management Console.
In the search bar, type "EC2" and select it from the dropdown list.
You will be taken to the EC2 Dashboard where you can manage your instances, volumes, security groups, and other resources related to EC2.

Explain the general difference between T2 Micro and XL.

In AWS, T2 and XL are two types of EC2 (Elastic Compute Cloud) instance families. T2 is a low-cost general-purpose instance family, while XL is a high-performance compute instance family.

The T2 family is designed for workloads that don't require high CPU performance consistently. These instances are ideal for small to medium-sized web applications, development and test environments, and small databases. T2 instances provide a balance of compute, memory, and network resources at a low cost, making them a popular choice for users who want to minimize their AWS bill.

On the other hand, the XL family is designed for compute-intensive workloads that require high performance and large amounts of memory. These instances are ideal for running large databases, high-performance computing (HPC), scientific modeling, and batch processing. XL instances provide dedicated CPU, memory, and network resources, making them capable of handling large-scale, high-traffic applications.

In summary, T2 instances are more suitable for general-purpose workloads that don't require high performance consistently, while XL instances are designed for compute-intensive workloads that require high performance and large amounts of memory. The cost of XL instances is typically higher than T2 instances due to the dedicated resources and higher performance.

Explain a “Compute Cycle” to a non-technical friend.

Let's say you have an EC2 instance running a web application. Each time a user visits your website and interacts with it, the EC2 instance uses compute cycles to process their requests and respond with the appropriate data. The more traffic your website gets, the more compute cycles the EC2 instance will need to handle those requests in a timely manner.

Different types of computing resources in AWS have different capabilities and limitations when it comes to compute cycles, which is why it's important to choose the right type and size of resource for your specific needs.

## Elastic Beanstalk

What is Elastic Beanstalk?

Elastic Beanstalk is a service for deploying and scaling web applications and services. Upload your code and Elastic Beanstalk automatically handles the deployment—from capacity provisioning, load balancing, and auto scaling to application health monitoring.

Describe the relationship between EC2 and Elastic Beanstalk.

Amazon Elastic Compute Cloud (EC2) and Elastic Beanstalk are both services provided by Amazon Web Services (AWS). EC2 is a scalable virtual computing environment that allows users to rent computing resources in the cloud. Elastic Beanstalk, on the other hand, is a Platform as a Service (PaaS) that streamlines the process of deploying web applications on AWS.

Elastic Beanstalk is built on top of EC2 and uses it as its underlying infrastructure. When you deploy an application to Elastic Beanstalk, it automatically provisions and manages the necessary EC2 instances and other AWS services required to run the application.

In other words, Elastic Beanstalk abstracts away the complexity of managing the underlying infrastructure, making it easier for developers to deploy and scale their applications without worrying about the underlying hardware. This allows developers to focus on building their applications, while AWS takes care of the infrastructure.

Name some benefits of using Elastic Beanstalk.

AWS Elastic Beanstalk makes it even easier for developers to quickly deploy and manage applications in the AWS Cloud. Developers simply upload their application, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.

[link-to-reading-notes](https://aws.amazon.com/ec2/).
[link-to-reading-notes](https://www.youtube.com/watch?v=lZMkgOMYYIg).
[link-to-reading-notes](https://www.youtube.com/watch?v=SrwxAScdyT0).


## Bookmark and Review

[link-to-reading-notes](https://www.youtube.com/watch?v=yIVXjl4SwVo).
[link-to-reading-notes](https://www.youtube.com/watch?v=l0DfHUWMjsU).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?