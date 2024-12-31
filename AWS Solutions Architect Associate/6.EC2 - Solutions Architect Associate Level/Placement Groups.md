- Sometimes you want control over the EC2 instance placement strategy
- Can be defined using placement groups 
The overall purpose of **placement groups** in AWS is to provide **control over how EC2 instances are deployed on the underlying AWS hardware**, tailoring the deployment to meet the specific needs of your application. Placement groups allow you to optimize performance, fault tolerance, and scalability based on your workload requirements.
#### Strategies
---
- Cluster: clusters instances into a low-latency group in a single AZ
- Spreads: spreads instances across underlying hardware - critical applications
- Partition: spreads instances across many different partitions within an AZ

**Cluster**:
- Pros: Great network (10 Gbps bandwidth between instances with enhanced networking enabled)
- Cons: if the AZ fails, all instances fail at the same time
- Used for dig data jobs that need to complete fast or application that needs extremely low latency and high network throughput 
![[Pasted image 20241229143630.png]]

**Spreads**:
All the EC2 instances are located on different hardware
- Pros: 
	- Can span across multiple AZs
	- Reduced risk to simultaneous failure
	- EC2 instances are on different physical hardware
- Cons:
	- Limited to 7 instances per AZ per placement group
- Use Case:
	- Needs to maximize high availability
	- Critical applications where each instance must be isolated from failure form each other
![[Pasted image 20241229143644.png]]
**Partition**:
Each partition represents a rack in AWS, distributed across many racks, safe from rack failure. There are up to 7 partitions for AZ, they can span across multiple AZs in the same region and there are up to 100s of EC2 instances. A partition failure can affect many EC2 but won't affect other partitions. We have partition information as metadata. USe cases are usually big data applications like Kafka
![[Pasted image 20241229144101.png]]