# IAM (Identity Access Management)
IAM stands for Identity and Acccess management and is a global service. A root account is created when you first log into the AWS console, it should NOT be used or shared. What we should do is create users, they can be people within our organization or tean and they can be grouped. Groups can only contain users and not any other groups. Note that users don't have to belong to a group, and the user can belong to multiple groups.
![image](https://github.com/user-attachments/assets/6b65982b-192f-40e6-839e-a92f434f398b)
- Best Practices: say that you should have everyone in a group
#### Permissions:
Users or groups can be assigned a JSON document called a policy, this policy essentially shows what resources these groups or users have access to. Note that AWS follows the least privilege principle, we don't give more permissions than a user needs.

![image](https://github.com/user-attachments/assets/6b509861-becd-4a00-ad00-3d19453a9dd1)

#### Policies:
Typing back to permissions, we can have policies within groups, but we can have what is called an inline policy which allows you to give policies to a specific user. See Fred.

![image](https://github.com/user-attachments/assets/ad9773b1-a20e-47b8-b737-45e47657e9bf)
![Pasted image 20241221091045](https://github.com/user-attachments/assets/20b860b0-06e9-4651-af3c-f25bac5bb307)

A policy structure consists of 
- Version: policy language version
- Id: an identifier for the policy
- Statement: one or more individual statements
A statement consists of 
- Sid: an identifier for the statement
- Effect: allows or denies access
- Principle: who this policy is applied to 
- Actions: list of actions this policy allows or denies
- Resource: list of resources to which the actions applied to
- Condition: Conditions for when this policy is in effect

# IAM Guidelinies & Best Practices
- Don't use the root account except for AWS account setup
- One physical user = One AWS user
- Assign users to groups and assign permissions to groups
- Create a string password policy
- Use and enforce use of MFA
- Create and use Roles for giving permissions to AWS services
- Use Access Keys for Programmatic Access
- To audit permissions of your account using IAM credentials report & IAM access advisor 
- Never share IAM users & Access Keys

# IAM Summary

- Users: Mapped to a physical user, has a password for AWS console 
- Groups: Contains users only
- Policies: JSON documents that outlines permissions for users or groups
- Roles: For EC2 Instances or AWS services
- Security: MFA + Password Policy
- AWS CLI: Manage AWS services using the command line
- AWS SDK: Manage AWS services using a programming language
- Access Keys: Access AWS using the CLI or SDK
- Audit: IAM credential reports & IAM access advisor 

