# Serverless 

Is serverless really mean that there is no server? Not exactly. At the end of the day, your code has to run somewhere, so servers do exist. Even when you build APIs using REST or GraphQL, they ultimately run on servers. For example, in Amazon Web Services, if you spin up an EC2 virtual machine, you explicitly configure the resources such as RAM (e.g., 5 GB) and storage (e.g., 500 GB), install the operating system (like Linux), set up runtimes such as Node.js, and deploy your application. In this case, you are fully responsible for managing the server, and you incur costs for as long as the server is running. If traffic increases, you may need to configure Auto Scaling groups to handle the load, which again requires manual setup and monitoring.

In any EC2-based setup, you are responsible for provisioning, configuring, and scaling the infrastructure based on your application’s needs. However, in a serverless approach using services like AWS Lambda, you only focus on writing and deploying your code. You do not need to worry about server management, OS installation, scaling, or capacity planning. AWS automatically decides the underlying infrastructure, including how much memory to allocate and how to scale your application based on incoming requests.

The main benefit is in the cost and operational model. In traditional systems, you pay for servers running 24/7, even when there is no traffic. In contrast, serverless follows a pay-per-use model. When a user invokes your API, your function is executed, returns a response, and then becomes idle. You are charged only for the number of invocations and the execution time, rather than continuous uptime. This makes serverless more efficient and cost-effective, especially for applications with variable or unpredictable traffic.

Now we were thinking of single user but suppose 1000+ users are trying to hit the same function or API (which again calls the function). so in that case serverless will do, it will create the copies of your code to handle those requests. that code is actually a AWS Lamda function. 

Checkout Lamda Pricing: <a href="https://aws.amazon.com/lambda/pricing/">Amazon Lamda </a>

and to handle all this the framework is also available <a href = "https://www.serverless.com/"> Serverless </a>


**Here you will have option for a Lamda Function.**
<hr>

<img width="1349" height="500" alt="image" src="https://github.com/user-attachments/assets/ff162d93-ff77-4b70-ae15-b643391c6e48" />

<hr>
