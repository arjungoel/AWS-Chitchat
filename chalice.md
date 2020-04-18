							    Chalice Serverless MicroFramework:-
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

- Getting started with Chalice
- Writing a sample application
- Deployment Pipeline

Prerequisites required:-

1. Python
2. Amazon API Gateway
3. AWS Lambda

Chalice is a python micro framework that is used for creating REST APIs. It has many good features:-

1. Declarative routing API -> It makes easy to create REST APIs in a declarative way and have it through a code first approach or a code driven approach.
2. Chalice provides CLI which helps in deployment, packaging and debugging etc.


Every Chalice App has an App Object that is at the module level and after that you can use one or more features in chalice for instance take 'routes' as an example.

To install chalice:-

pip install chalice

To check the version of chalice:->  chalice --version


chalice --help will give you a list of all the important commands required to create chalice app and further more processes.


chalice deploy -> It go through and figure out all the resources it needs to deploy. It will generate an IAM role for us, it will create the deployment package which has all of our
dependencies that we need including the chalice runtime. It will also create a lambda function for usand then finally it will create the API Gateway Portion which is the swagger document and 
then an actual REST API.

When you run this command you will get 2 important things:-
1. Lambda ARN
2. REST API URL

In order to work with HTTP/HTTPS requests:-> pip install httpie
you can also use curl.

In order to do http request and fetch the output:- http REST API URL
