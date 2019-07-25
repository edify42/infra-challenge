# Infra-challenge

Single application on AWS example. This example will consist of:

* VPC config, firewalls and security groups
* Autoscaled EC2 instances running a simple web application behind a LB
* AWS RDS Mysql Aurora instance
* S3 bucket with Ansible bootstrap config
* IAM roles EC2 instances

A sample NodeJS application will read/write the the Aurora DB.
This example roughly translates to a traditional old school LAMP stack.

## Preconfiguration

In AWS SSM, we'll store the RDS default user and password to keep it out of
the CF template

## Directories

`./infrastructure` contains the IaaC files to build whats needed.
`./app` contains the NodeJS source code for the webserver.
`./bootstrap` contains the Ansible files to configure the EC2 instances

### Infrastructure

Divided into the Cloudformation templates below

#### Networking

Simple VPC configuration, with routing logic for external internet access

#### EC2 ASG RDS, S3 and IAM policies

#### Something else?

## live example

A URL will be supplied which shows of the usage of the application.
