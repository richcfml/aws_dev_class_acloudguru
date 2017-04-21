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

	- Regions - place in the world where AWS has resources 14. consist of 2 or more availability zone
	- Availability Zones - 38 - data center or a collection of data centers
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



















