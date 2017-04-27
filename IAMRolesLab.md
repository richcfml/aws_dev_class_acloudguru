## IAM Roels Lab

### Notes
The ec2 role that is provision with the ec2 instance can't be removed or can't add a new role. What can be done is to add new policies to the role, the policies are effective immediately.

Roles are more secure than storing access key and secret access key in ec2 instances
Roles are easier to manage
Roels can only be assigned when the EC2 instance is being provisioned - This has changed as of Feb 2017 and it is now change or add new roles to a running EC2 instance 
Roles are universal, you can use them in any region