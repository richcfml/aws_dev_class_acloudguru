IAM (Identity Access Management) - Universal and does not apply to regions

IAM allows you to mange users and thier level of access to he AWS Console.

### Provides

centralized control of aws acct
shared access to the aws acct
provides granular permissions
allows identity fedrataion with active directory, facebook, linkedin, etc and it allows the user of those services as a single sign on as well as the use of your aws resources for apps that use facebook or instagram etc.
multifactor authentication
provide temp access to users, devices and services when and where needed
password rotation and policies
integrates with many aws services
Support PCI DSS compliance

### Critical Terms

User is all end users
Group is a collection of users under one set of permissions
Roles is something you create and assign them to AWS resources
Policies a way to create a document with permissions

### Lab1


### Federation

can you authenticate with AD and the answer is yes and it is using SAML
are you auth to AD and get a temp credential or first get a temp credential and then via aws auth to AD and the correct answer is the first one, auth to AD and get temp cred first

### Web Identity Federation with Mobile Apps

Facebook, linkedim, Google, amazon acct and to setup it needs code. More info at aws.amazon.com/articles/4617974389850313

the methodology is that when sign in to aws there is an auth token ad then in aws you get a temp sec credentials with a trust policy, which is the rule set for access, a provider which will be the service, such as facebook, a RoleARN (Amazon Resource Name) and a web token, then a call to AsumeRoleWithWebIdentity needs to be done to actually access the resources.

Understand the process for the exam






