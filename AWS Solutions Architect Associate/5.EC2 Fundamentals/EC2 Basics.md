Elastic Compute Cloud = Infrastructure as a service
Mainly consists in the capability of: 
- Renting virtual machines (EC2)
- Storing data on virtual drives (EBS)
- Distributing load across machines (ELB)
- Scaling the services using an auto-scaling group (ASG)
Knowing EC2 is fundamental to understand how the cloud works

#### Sizing & Configuration options
---
- Operating System
- Compute power & cores
- RAM
- Storage space
	- network attached
	- hardware attached
- Network card: speed of the card, public IP address
- Firewall Rules: Security group
- Bootstrap script 

#### EC2 User Data
---
It is possible to bootstrap our instances using an EC2 User data script 
- Bootstrapping means launching commands when a machine starts
- The script is only run once at the instance first start 
- EC2 user data is used to automate boot tasks such as 
	- installing updates
	- installing software
	- downloading common files from the internet
	- Basically anything we can think of
