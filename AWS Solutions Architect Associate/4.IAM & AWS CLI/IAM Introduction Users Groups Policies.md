#### IAM
---
- IAM stands for Identity and Access Management, Global Service
- The root account is created by default, it shouldn't be used or shared
- We should create users and they are people within our organization, and can be grouped
- Groups only contain users, not other groups
- Users don't have to belong to a group, and the user can belong to multiple groups
![[Pasted image 20241221085554.png]]
- Now not all users have the belong to a group, for example Fred, but it is under best practices to have everyone in a group
**Permissions**:
- Users or groups can be assigned a JSON document called a policy
 ![[Pasted image 20241221085632.png]]
- So the people in this group would have access to EC2, elastic cloud, and cloud watch
- These policies help us define the policies define the permission of the users
- In AWS we apply the least privilege principle, we don't give more permissions than a user needs