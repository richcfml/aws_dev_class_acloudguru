EC2 (Elastic Compute Cloud)

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

Family - D2
Specialty - Dense Storage
Use Case - Fileservers, data warehousing, hadoop
--
Family - R4
Specialty - Memory Optimized
Use Case - Memory intensive Apps/DBs
--
Family - M4
Specialty - General Purpose
Use Case - Application Servers
--
Family - C4
Specialty - Compute Optimized
Use Case - CPU intensive Apps/DBs
--
Family - G2
Specialty - Graphics Intensive
Use Case - Video Encoding, 3d application streaming
--
Family - I2
Specialty - High Speed storage
Use Case - NoSQL DBs, data warehousing
--
Family - F1
Specialty - Field Programmable Gate Array
Use Case - Hardware acceleration for your code
--
Family - T2
Specialty - Lowest cost, general purpose
Use Case - Web server, small DBs
--
Family - P2
Specialty - Graphics, general purpose gpu
Use Case - machine learning, bit coin mining etc
--
Family - X1
Specialty - Memory optimized
Use Case - SAP Hana, Apache Spark

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

