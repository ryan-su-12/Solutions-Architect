#### Inheritance
---
![[Pasted image 20241221091013.png]]
So we can have policies in groups, see developers or operations, but we can also have what is called an inline policy, this allows you to give policies to a specific user

#### Policy Structure
---
![[Pasted image 20241221091045.png]]
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
