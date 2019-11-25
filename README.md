# How to Build a Serverless Backend with AWS Lambda and Node.js

*Get familiar with function-as-a-service (FaaS), deploy a demo on a AWS Lambda serverless computing platform, hook up a MongoDB database-as-a-service to a serverless REST API, and more.*

[origin](https://medium.com/crowdbotics/how-to-build-a-serverless-backend-with-aws-lambda-and-nodejs-e0d1257086b4)

Serverless architecture is a cloud computing execution model where a cloud provider like AWS, Azure or Google Cloud is used to deploy backend or server-side code. In comparison to traditionally deployed web applications, in serverless architecture, the developer does not has to maintain the servers or the infrastructure. They only have to pay a subscription to the third party vendor whereas the vendor is responsible to handle the operation of the backend logic of a server along with scalability, reliability, and security.

There are two ways a serverless architecture can be implemented in order to deploy your server-side code. First one is Backend as a Service or BaaS. A good example of this is Firebase which you can often see in conjunction between a web or a mobile application to a database or providing user authentication.
What we are going to focus in this article is called Function as a Service or FaaS. With FaaS, the server code is run inside containers that are usually triggered by common events such as HTTP requests from the client, database operations, file uploads, scheduled events and so on. The code on the cloud provider that is deployed and getting executed is in the form of a function.

In FaaS, these functions are deployed in modular form. One function corresponds to each operation, thus eliminating the rest of the code and time spent on writing boilerplate code for setting up a server and data models. These modular functions can further be scaled automatically and independently. This way, more time can be spent on writing the logic of the application that a potential user is going to interact with. You do not have to scale for the entire application and pay for it. Common use cases of FaaS so far have been implemented are scheduled tasks (or cron jobs), automation, web applications, and chatbots.

Common FaaS service platform providers are:

- AWS Lambda
- Google Cloud Functions
- Microsoft Azure Functions
- Apache OpenWhisk

In the following tutorial, we are going to create a demo to deploy on a serverless infrastructure provider such as AWS Lambda.
