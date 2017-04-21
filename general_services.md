# Overview of all AWS Services

To pass the exam for Developer Assocaite you need to know about

	- messaging
	- Security & Identity
	- Management tools
	- Storage
	- Databases
	- Networking & content delivery
	- Compute
	- AWS Global Infrastructure

# AWS Global Infrastructure

It is the physical pieces that AWS runs on and it is broken down into three different parts

	- Regions - place in the world where AWS has resources 16. consist of 2 or more availability zone. Further info at https://aws.amazon.com/about-aws/global-infrastructure/
	- Availability Zones - 38 - data center or a collection of data centers - Availability Zones are distinct locations within an AWS region that are engineered to be isolated from failures.
	- edge locations - over 66 - is a CDN end point for cloud front

# Network and Content Delivery

### VPC - Virtual Private Cloud
Important part of the exam. 
It is like a virtual data center where resources are deployed to. 

### Route53
DNS service

### Cloud Front
Networking and content delivery network

### Direct Connect
A way to connect your office or physical data centers to AWS with a dedicated line


# Compute

### EC2
Elastic Compute Cloud and it is just like VMs in the cloud

### EC2 Container Services
It is high scalable and preformance to manage docker containers

### Elastic Beanstalk
Service that provides the ability to deploy code and AWS manage all of the infrastructure needed for the code

### Lambda
Serverless to upload the code to respond to events

### lightsail
Out of the box cloud to deploy different solutions such as wordpress

### Storage

S3 is for object base storage, such as pictures or word documents.
Glacier is a backup storage for S3 and it is normally for long term storage that does not require fast access. It may take about 3 to 4 hours to retreive data
EFS is a Elastic File Service and it is a block base storage where you can store dbs or apps and it can be shared among several ec2s
Storage Gateway is a VM that you install on prem and it is to connect directly to S3

### Databases

RDS is relational database services that include many database engines
DynamoDB is a non-relational database service, NoSQL and very scalable and high performance
Redshift is the datawarehouse solution 
Elasticache is a way to cache data 

### Migration

Snowball is an appliance that gives you a way to move data into the cloud
DMS is a database migration services and allows to migrate db from one source to another point and can migrate from one engine to another, eg. Oracle to Aurora
Server migration Service (SMS) it targets VMWare VMs to replicate them and migrate them as needed

### Analytics

Athena is a way to allow sql queries on files stored in s3
Elastic Map Reduce is use for big data processing such as log analysis
Cloud Search gives the ability to manage and create search capabilities for an application
Elastic Search same as cloud search but with non Amazon base but third party libraries
Kinesis streams and analyzes large amount of data
Data pipeline is a service that allows you to move data from one point to another
Quick Sight is a business analytics tool

### Security & Identity

IAM is the service for authentication and permissions, groups etc.
Inspector is an agent that it is install in the virtual machines to do security reporting
Certificate Manager is for a free ssl certs for domain names
Directory Services is a way to connect to AD from AWS
WAF is the web application firewall and it give application level protection
Artifacts is a way to get the documentation in the AWS console for ceretifications such as PCI DSS or ISO documentation

### Management tools

Cloud watch is use to monitor performace of the aws environment
Cloud Formation is a way to turn your infrastructure into code. It is a document that describe your environments and deploy them from that document or templates
Cloud Trail is a way to audit the aws resources and changes to them
Opsworks is a way to automate deployments using shift
Config Manager is a way to monitor environments and when it breaks or have problems and set alerts 
Service Catalog is design for large enterprise to setup rules on services in aws and their use and permissions to them
Trusted Advisor is a tool to provide a scan of enviornment and provide tips for imporvement

### Application Services

Step Functions is a way to view what is going in your app or microservices it is using
SWF simle workflow flow is a way to automate tasks such as workflow for shipping items 
API Gateway is a door that allows you to create APIs at scale for backend data and services
AppStream is a way to stream desktop apps to users
Elastic Transcoder is a way to format video for diferent devices and formats

### Developer Tools

CodeCommit is a git storage 
CloudBuild is a way of compiling your code
CodeDeploy is a way of deploying the code to EC2
CodePipeline is a way to track all of the version of your code in different environments

### Mobile Services

Mobile Hub confiure design features for mobile apps such as authentication and storage
Cognito is a way to sign up and sign in to apps with services such as gmail
Device Farm is a way to improve apps by testing apps in physical devices
Mobile Analytics is a way to analyze mobile data
Pinpoint is a way to enable and engage with users. Similar to google analytics

### Business Productivity

WorkDocs a way to store securily work documents
WorkMail is like Exchange for AWS

### IoT

It is a way to keep and track millions of devices

### Desktop and App streaming

WorkSpaces is a way of having a desktop in the cloud like a VDI
AppStream 2.0 it is a way to stream desktop applications to users

### Artifical Intelligence

Read book Superintelligence by Nick Bostrom
Alexa is a service that talks to Lambda, it is based on Lex 
Polly is a text to speach service
Machine Learning is a way to provide a end result and the service analyzes the info and predict future interactions such as buying patterns
Rekognition is a service that will give you information on a picture such as the elements on the picture like, mountains as well as face recognition

### Messaging
SNS is simple notification services to notify in various ways
SQS is a way to decouple application. it is a queue system to create jobs with tasks
SES is simple email service and a way to sending and recieving email














