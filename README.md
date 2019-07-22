# infra-challenge

single application on AWS example. This example will consist of:

* API Gateway for incoming web requests
* Lambda to handle the service traffic
* IAM roles for lambda to access DynamoDB

A sample NodeJS application will read/write the the DynamoDB.
This example roughly translates to a traditional old school LAMP stack.

## directories

`./infrastructure` contains the IaaC files to build whats needed.
`./app` contains the NodeJS source code for the webserver.

## live example

A URL will be supplied which shows of the usage of the application.
