- An EFS is a managed NFS (network file system) that can be mounted on many EC2
- EFS works with EC2 instances in multiple availability zones
- Highly available, scalable, and expensive
Essentially a scalable, network-based file storage solution designed to grow or shrink automatically as you add or remove data
![[Pasted image 20241230183557.png]]
**Use cases**
- Content management, web serving, data sharing, WordPress 
- Uses security group to control access to EFS 
- Only compatible with Linux based AMI
- File system scales automatically, pay-per-use, don't need to plan for capacity

**Performance & Storage Classes**:
- EFS Scale
	- 1000s of concurrent NFS clients
	- Grows to petabyte scale network file system automatically
- Performance Mode:
	- General purpose is for latency sensitive cases
	- Max I/O: Higher latency, throughput, highly parallel
- Throughput Mode (amount of data that can be transferred)
	- Busting
	- Provisioned 
	- Elastic - Automatically scales throughput up or down based on workloads
**Storage Classes**:
- Standard: for frequently accessed files
- Infrequent Access: Cost to retrieve files, lower price to store
- Archive: rarely accessed data
We can implement lifecycle policies to move files between storage tiers
