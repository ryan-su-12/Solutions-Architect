**EBS Volume**:
- An EBS (Elastic Block Store) volume is a network drive you can attach to your instances while they run 
- It allows your instances to persist data, even after their termination
- They can only be mounted to one instance at a time 
- They are bound to a specific availability zone
Essentially network USB sticks
**Definition**:
It is a network drive, it uses the network to communicate the instance, which means there might be a bit of latency, it can be detached from an EC2 instance and attached to another quickly. However, its locked to an availability zone, to bypass this you need to snapshot it. Finally you must provision the capacity. 
![[Pasted image 20241230103858.png]]
**Delete on termination attribute**:
![[Pasted image 20241230103948.png]]
- Controls the EBS behvaiour when an EC2 instance terminates
	- By default, the root EBS volume is deleted
	- By default, any other attached EBS volume is not deleted
	- Used when we want to preserve the root volume when an instance is terminated

#### EBS Volume Types
---
EBS volumes come in 6 types
- gp2 / gp3 (SSD): General purpose SSD volume that balances price and performance for a wide variety of workloads
- io 1/ io2 Block Express (SSD): Highest-performance SSD volume for mission-critical low-latency or high-throughput workloads
- st I (HDD): Low cost HDD volume designed for frequently accessed, throughput-intensive workloads
- sc i (HDD): Lowest cost HDD volume designed for less frequently accessed workloads 
EBS volumes are characterized in size, throughput I/O operations per section 

One gp2/gp3 and io 1/ io 2 can be used as boot volumes

**General Purpose SSD**:
These provide cost effective storage, low-latency, it has system boot volumes, virtual desktops, development and test environments and are in the range of 1 GB to 16 TB
gp3:
- Baseline of 3000 I/O operations per second and throughput of 125 MiB/s
- Can increase up to 16000 and 1000 MiB/s respectively
- You can independently set the IOPS
gp2:
- Small gp2 volumes can burst IOPS to 3,0000
- Size of the volume and IOPS are linked, Max IOPS is 16,000
- 3 IOPS per GB, means at 5,334 GB we are at the max IOPS

**Provisioned IOPS (PIOPS) SSD**:
These are useful for critical business applications with sustained IOPS performance or applications that need more than 16,000 IOPS. This makes it great for databases workloads
- io 1( 4GB - 16TB):
	- Max PIOPS: 64,000 nitro for EC2 instances & 32,000 for other
	- Can increase PIOPS independently from storage size
- io 2 Block Express ( 4GB - 64 TB):
	- Sub-millisecond latency
	- Max PIOPS: 256,000 with an IOPS: GB ration of 1,000 to 1
**Hard Disk Drives (HDD)**:
- Cannot be a boot volume
- 125 GB to 16 TB
- Throughput Optimized is good for Big data, data warehouses, log processing 
**Cold HDD (sc1)**:
- For data that is infrequently accessed
- Scenarios where lowest cost is important
![[Pasted image 20241230182255.png]]