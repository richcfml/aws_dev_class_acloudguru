## Bash Scripting Lab

The script below can be added in the launch of an EC2 instance under the additional area.
#!/bin/bash
yum update -y
yum install httpd -y
service httpd start
chkconfig httpd on
aws s3 cp s3://mywebsitebucket-richacloudguru/index.html /var/www/html