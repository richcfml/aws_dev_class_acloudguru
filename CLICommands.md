## CLI Commands

### Commands to remember and know for the exam

aws ec2 describe-instances - command to describe the current available instances
aws ec2 describe-images - command to describe the available images that can be use to provision a new instance
aws ec2 run-instances - command to create(launch) a new instance, Must have a key pair and a security group

DO NOT CONFUSE start-instances with run-instances. The start-instances is use to start an existing instance.

### Docs

http://docs.aws.amazon.com/cli/latest/reference/ec2/

Remembe the command for terminate-instances

aws ec2 terminate-instances --instance-ids i-1234567890abcdef0 where i-1234567890abcdef0 is the instance name