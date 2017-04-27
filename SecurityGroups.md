## Security Groups

### Lab

it is a virtual firewall and controls traffic access to the EC2 instance. 

Rules are stateful and it will automatically back out if it exists in the inbound rules even if there is no rules in the outbound rule

All inbound traffic is blocked by default
All outbound traffic is allowed by default
Changes to security groups take effect immediately
You can have more than one EC2 instannce to a sec groiup
You an have multiple sec group attached to EC2 instances
You cannot block specific IP address using Sec groups instead use Network Access Control Lists
You can specify allow rules but not deny rules
