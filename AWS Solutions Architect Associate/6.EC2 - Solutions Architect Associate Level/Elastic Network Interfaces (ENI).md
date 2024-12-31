An **Elastic Network Interface (ENI)** in AWS is a **virtual network card** that you can attach to an Amazon EC2 instance. It enables an instance to communicate within a Virtual Private Cloud (VPC) and with other resources. The ENI serves as a building block for managing networking within AWS and offers features like **multiple IP addresses**, **high availability**, and **flexibility** for networking setups.

- Logical component in a VPC that represents a virtual network card
- Each ENI can have the follow attributes
	- Primary private IPv4, one or more secondary IPv4
	- One elastic IP per private IPv4
	- One public IPv4
	- One or more security groups
- You can create ENI independently and attach them on the fly on EC2 instances for failover
- Bound to specific AZ