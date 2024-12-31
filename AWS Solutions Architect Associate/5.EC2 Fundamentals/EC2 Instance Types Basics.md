**Naming Convention**:
$$\text{m5.2xlarge}$$
- m: This is the instance class
- 5: This is the generation (aws improves them over time)
- 2xlarge: This is the size within the instance class
#### EC2 Instance Types
---

**General Purpose**:
- Great for diversity of workloads such as web servers or code repositories
- Balance between:
	- Compute
	- Memory
	- Networking
- In this Udemy course, t2.micro is used which is a general purpose EC2 Instance
![[Pasted image 20241227172221.png]]

**Compute Optimized**:
- Great for compute-intensive tasks that required high performance processors
	- Batch processing workloads
	- media transcoding
	- High performance web servers
	- High performance computing (HPC)
	- Scientific modeling & machine learning
	- Dedicated gaming servers 
![[Pasted image 20241227172403.png]]

**Memory Optimized**:
- Fast performance for workloads that process large datasets in memory
- Use cases
	- Higher performance, relational/non-relational databases
	- Distributed web scale cache stores
	- In-memory databases optimized for Business intelligence
	- Applications performing real-time processing o big unstructured data
![[Pasted image 20241227172600.png]]

**Storage Optimized**:
- Great for storage-intensive tasks that required high, sequential read and write access to large data sets on local storage
- Use cases
	- High frequency online transaction processing systems 
	- Relational & NoSQL databases
	- Cache for in-memory databases
	- Data Warehousing applications
	- Distributed file systems 
![[Pasted image 20241227172803.png]]

#### Example
---
![[Pasted image 20241227172820.png]]
