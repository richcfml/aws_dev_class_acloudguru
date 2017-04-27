# EC2 (Elastic Compute Cloud)

is a web service that provides resizable compute capacity in the cloud

### Options

- On Demand allow you to pay a fixed rate by the hour with no commitments
- Reserved provides you a capacity reservation and offer a significant discount on the hourly charge for an instance. 1year or 3 year terms
- Spot enables you to bid on whatever price you want for instance capacity, providing even greater savings
- Dedicated Hosts - physical EC2 server dedicated for your use. pay bu the hour

#### On Demand

Users that want the low cost and flexibility of amazon ec2 without up-front payment or long-term commitment. ALso use for applications with short-tem, spiky or unpredictable workload that can't be interrupted as well as applications being developed or tested in EC2 for the first time

#### Reserved

Applicaations with steady state or predicable usage and/or required reserved capacity and the user is able to pay up-front and reduce cost

#### Spot

Spot is the price at any given time for the resource. Applications that have flexible start and end times and only feasable at very low compute prices and users for urgent compute needs for large amount of additional capacity. 

Exam Tip, spot intance are terminated by Amazon EC2 and no charge for the partial hour of usage, but if the person terminates the instance the user will be charged for any hour in which the instance ran.

#### Dedicated Host

useful for regulatory requirements that do not support multitenant virtualization and for licensing that does not support multi-tenancu or cloud deployments. Can be purchased hourly and as a reservation can get up to 70% off

### Instance Types

| Family        | Specialty           | Use Case  |
| ------------- |:-------------| :-----|
| D2 |  Dense Storage | Fileservers, data warehousing, hadoop |
| R4 | Memory Optimized | Memory intensive Apps/DBs |
| M4 | General Purpose | Application Servers |
| C4 | Compute Optimized | CPU intensive Apps/DBs |
| G2 | Graphics Intensive | Video Encoding, 3d application streaming |
| I2 | High Speed storage | NoSQL DBs, data warehousing |
| F1 | Field Programmable Gate Array | Hardware acceleration for your code |
| T2 | Lowest cost, general purpose | Web server, small DBs |
| P2 | Graphics, general purpose gpu | machine learning, bit coin mining etc |
| X1 | Memory optimized | SAP Hana, Apache Spark |

Tip to learned them, DR Mc GIFT PX
D for Density
R for RAM
M for main chose for general purpose apps
C for Compute
G for graphics
I for IOPS
F for FPGA (field programmable gate arrays)
T cheap general purpose (think t2Miccro)
P for Graphics (think Pics)
X for Extreme Memory

### EBS

Allows you to create storage volumes and attached them to the EC2 instances

Types:
General Purpose SSd (GP2)
- balance for price and performance
- ratio is 3 IOPS per GB with up to 10,000 IOPS with bust up to 3000 IOPS for extended period of time for volumes undeer 1GB.

Provisioned IOPS SSD (IO1)
- design for I/O intenisve app such as large relational DBs or NoSql
- Use if need more than 10,000 IOPS

Throuhput Optimized HDD (ST1)
- Use for Big data, data warehouse or log processing
- Use for data thaat is stored in sequence
- Cannot be a boot valume

Cold HHD (SC1)
- Lowest cost storage for infrequent access workloads
- Use for things such as file server
- Cannot be boot valume

Magnetic (standard)
- Lowest cost per GB of all EBS volume that is bootable
- Ideal for workload whre data is access infrequently
- Use for applications where lowest cost storage is important

### Exam Tips

#### Know difference of pricing models
- On Demand
- Spot
- Reserved
- Dedicated Hosts

#### Rememer with spot instance
- If you terminate the instance, you pay for the hour
- If AWS terminate you get the hour when it was terminated for free

#### EBS
- SSD, General Purpose - GP2 - up to 10,000 IOPS
- SSD Provision IOPS - IO1 -  More than 10,000 IOPS up to 20,000 
- HDD, Throughput Optimized - ST1 - requent accessed workloads - NOT BOOTABLE
- HDD, Cold - SC1 - less frequent accessed data - NOT BOOTABLE
- HDD, Magnetic - Standard, cheap, infrequent acess storage

**You cannot mount 1 EBS volume to multiple EC2 instances, instead use EFS**

REMEMBER EC2 Instances


### LAB

**One Subnet equalts One Availability Zone**

**Status Checks**
- System Status Checks - verify that instance is reachable
- Instance Status Checks - check that traffic can get to the instance