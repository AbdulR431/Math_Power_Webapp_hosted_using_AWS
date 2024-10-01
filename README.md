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
Then tested and deployed the code necessary to calculate the value of power of a base.

# Step 3:

Built the RestApi using AWS API Gateway with method Post, then Lambda is attached to the method.
Enabled CORS
Use of CORS: CORS (Cross-Origin Resource Sharing) is a mechanism that allows web pages to make requests to a server on a different domain than the one from which the page originated. By enabling CORS in your AWS API Gateway, you're essentially granting permission for your API to be accessed from different domains, allowing for more flexible and integrated web applications.
As our web-application is deployed using Amplify and We use AWS Lambda to calculate the value of power of a base, enabling cors triggers the lambda function and providers the user output.
Then the API is Deployed.
Invoke Url is saved.

# Step 4:

An AWS Dynamodb Table is created and its arn(amazon resource name) is stored.

![creation of the Dynamodb table](https://github.com/AbdulR431/Math_Power_Webapp_hosted_using_AWS/blob/main/Project-Images/dynamodb%20usage.PNG)

# Step 5:

Now Using AWS IAM we have to give necessary permissions to the Lamba in order to ensure Lambda is able to store the calculated result in the dynamodb table.
Attached a JSON policy in which arn of the dynamodb table is pasted.

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

