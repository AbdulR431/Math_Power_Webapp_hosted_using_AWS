# Math_Power_Webapp_hosted_using_AWS
A Small Project Built by me using AWS services.
A simple web application Built using AWS, which calculates the value of power of a base.

![Web-application](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/AWS%20project.PNG)

# AWS Services Used:

![AWS Services Used in project](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/AWS%20Services%20Used.PNG)

-> AWS Amplify

-> AWS API Gateway

-> AWS Lambda

-> AWS Dynamodb

-> AWS IAM.

# Steps:

# Step 1:

html file is Deployed on the web using the AWS Amplify.

![Deployement of the web-application using Amplify](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/Amplify%20usage.PNG)

Breif Use of the Amplify:
AWS Amplify is a fully managed development platform that allows you to build, deploy, and host web and mobile applications. It provides a set of tools and services that simplify the process of building and managing cloud-powered applications.

key benefits of using AWS Amplify:

Rapid application development: Amplify provides pre-built components and services that can be used to quickly build and deploy applications. This can save you time and effort, especially if you are new to cloud development.
Scalability: Amplify is designed to scale with your application's needs. This means that you can easily add or remove resources as your application grows.
Reliability: Amplify is a highly reliable platform that is backed by AWS's global infrastructure. This means that you can be confident that your application will be available to your users whenever they need it.
Security: Amplify provides a number of security features to help protect your application and data. These features include data encryption, authentication, and authorization.
Cost-effective: Amplify is a cost-effective way to build and deploy applications. You only pay for the resources that you use.

Here are some of the specific features of AWS Amplify:

Frontend development: Amplify provides a framework for building web and mobile applications. This framework includes components for common UI elements, such as buttons, forms, and navigation menus.
Backend development: Amplify provides a set of services that can be used to build and manage the backend of your application. These services include data storage, authentication, and push notifications.
Deployment: Amplify makes it easy to deploy your application to the cloud. You can deploy your application with a single click, and Amplify will handle all of the configuration and deployment tasks for you.
Hosting: Amplify provides a hosting platform for your application. This means that you don't have to worry about managing your own servers or infrastructure.
Analytics: Amplify provides a set of analytics tools that can help you understand how your application is being used. This information can be used to improve your application's performance and user experience.
Overall, AWS Amplify is a powerful and flexible platform that can be used to build and deploy a wide variety of web and mobile applications. If you are looking for a way to simplify the process of building and managing cloud-powered applications, Amplify is a great option to consider.

# Step 2:

Created a Lambda function of type python.

Brief Use of AWS Lambda:

AWS Lambda is a serverless computing platform that lets you run code without provisioning or managing servers. You pay only for the compute time you consume. With Lambda, you can upload your code and configure it to run in response to various triggers, such as API calls, file uploads, or scheduled events.   

Key benefits of using AWS Lambda:

Serverless: No need to manage servers or infrastructure.
Scalable: Lambda automatically scales your code to handle changes in demand.
Cost-effective: Pay only for the compute time you use.
High availability: Lambda is designed for high availability and fault tolerance.
Integration: Easily integrates with other AWS services and third-party applications.

Common use cases for AWS Lambda:

API development: Create RESTful APIs without managing servers.
Data processing: Process large datasets at scale.
Event-driven applications: Trigger actions based on events from other services (e.g., S3, Kinesis).
Real-time applications: Process data in real-time.
Microservices architecture: Build and deploy small, independent services.
In essence, AWS Lambda provides a flexible and efficient way to run code without the overhead of managing servers, making it a popular choice for building scalable and cost-effective applications.
Then tested and deployed the code necessary to calculate the value of power of a base.

# Step 3:

Built the RestApi using AWS API Gateway with method Post, then Lambda is attached to the method.

Brief about AWS API Gateway:
AWS API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure RESTful APIs at any scale. It acts as a front door for applications that access backend services.   

Key features and benefits of AWS API Gateway:
RESTful APIs: Create and manage RESTful APIs with various HTTP methods (GET, POST, PUT, DELETE, etc.).
API Gateway proxy integration: Easily integrate with backend services like AWS Lambda, AWS EC2, or HTTP endpoints.
API Gateway Lambda proxy integration: Directly integrate with AWS Lambda functions for serverless computing.
API key management: Secure your APIs with API keys to control access and usage.
Usage plans: Create usage plans to limit API usage and throttle requests.
Custom authorizers: Implement custom authorization mechanisms for fine-grained access control.
Caching: Improve performance by caching API responses.
Monitoring and analytics: Track API usage, latency, and errors through built-in metrics and logs.
Deployment stages: Create different deployment stages (e.g., dev, test, prod) for managing API versions.

Use cases for AWS API Gateway:
Mobile and web applications: Expose backend services to mobile and web apps.
IoT devices: Provide APIs for IoT devices to communicate with cloud-based services.
Microservices architecture: Create APIs for microservices to interact with each other.
Serverless applications: Build serverless applications using Lambda and API Gateway.
In summary, AWS API Gateway simplifies the process of building, managing, and securing APIs, making it a valuable tool for developers building cloud-native applications.

Enabled CORS
Use of CORS: CORS (Cross-Origin Resource Sharing) is a mechanism that allows web pages to make requests to a server on a different domain than the one from which the page originated. By enabling CORS in your AWS API Gateway, you're essentially granting permission for your API to be accessed from different domains, allowing for more flexible and integrated web applications.
As our web-application is deployed using Amplify and We use AWS Lambda to calculate the value of power of a base, enabling cors triggers the lambda function and providers the user output.
Then the API is Deployed.
Invoke Url is saved.

# Step 4:

An AWS Dynamodb Table is created and its arn(amazon resource name) is stored.

Brief about AWS Dynamodb:
AWS DynamoDB is a fully managed NoSQL database service that provides fast and reliable performance for any scale. It is a key-value store that offers high availability, low latency, and automatic scaling.

Key features and benefits of DynamoDB:
High performance: Delivers consistent low latency performance, even at massive scale.
Scalability: Automatically scales to handle any workload, from small to massive.
Durability: Provides strong consistency and durability for your data.
Flexibility: Supports both document and on-demand capacity modes.
Global tables: Replicate data across multiple regions for low-latency access.
Secondary indexes: Create secondary indexes for efficient querying on non-primary key attributes.
Stream processing: Capture and process data changes in real-time using DynamoDB Streams.
Serverless: No need to manage servers or infrastructure.

Use cases for DynamoDB:
Mobile and web applications: Store and retrieve data for mobile and web apps.
Games: Store game data, user profiles, and leaderboards.
IoT applications: Store and process data from IoT devices.
Real-time analytics: Process data in real-time for analytics and reporting.
Serverless applications: Use as a data store for serverless applications built on Lambda and API Gateway.
In summary, DynamoDB is a powerful and flexible NoSQL database service that can handle a wide range of workloads, making it a popular choice for building scalable and reliable applications.

![creation of the Dynamodb table](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/dynamodb%20usage.PNG)

# Step 5:

Now Using AWS IAM we have to give necessary permissions to the Lamba in order to ensure Lambda is able to store the calculated result in the dynamodb table.
Attached a JSON policy in which arn of the dynamodb table is pasted.

Brief about AWS IAM:
AWS Identity and Access Management (IAM) is a service that allows you to securely manage users, groups, and permissions in AWS. It provides granular control over who can access your AWS resources and what actions they can perform.

Key features and benefits of IAM:
Users: Create and manage AWS users with unique credentials.
Groups: Organize users into groups for efficient permission management.
Roles: Assign permissions based on roles, allowing temporary access to AWS resources.
Policies: Define policies to specify what actions users or groups can perform on AWS resources.
Multi-factor authentication (MFA): Enhance security by requiring MFA for user sign-in.
Access keys: Generate and manage access keys for programmatic access to AWS services.
Federation: Integrate with external identity providers (IdPs) for single sign-on (SSO).
IAM roles for services: Assign IAM roles to AWS services to grant them permissions to access resources.
Conditional permissions: Apply conditions to policies based on attributes like time, location, or resource tags.

Use cases for IAM:
User management: Manage user accounts and permissions within your AWS environment.
Access control: Implement granular access control for AWS resources.
Security best practices: Enforce security best practices by using IAM features like MFA and conditional permissions.
Cross-account access: Grant access to resources in other AWS accounts using IAM roles.
Integration with third-party applications: Integrate with external identity providers for SSO.

In summary, IAM is a crucial service for managing user access and security in AWS, ensuring that only authorized users can perform specific actions on your AWS resources.

![Attached policy](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/JSON%20policy.PNG)

# Step 6:

Now in the final step Added the API Invoke url to the html file which ensure its connection to the API.

![API Gateway Endpoint](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/Api%20Gateway%20Endpoint.PNG)

Then Again deploy the changes using AWS Amplify.

# Result:

Finally our Simple Web-application is ready to be used.

![Final Result](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/AWS%20project%20result.PNG)

# Thank YOU
# The End

