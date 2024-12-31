**On-Demand Instances**:
- Short workload, predictable pricing, pay by second
- Recommended for short--term and un-interrupted workloads, where you can't predict how the application will behave 

**Reserved ( 1 & 3 Years)**: 
- Reserved instances - long workloads
- Convertible Reserved Instances - long workloads with flexible instances
- Recommended for steady-state usage applications (like a database)
- Convertible Reserved Instance
	- Can change the EC2 instance type, instance family, OS, scope and tenancy

**Savings Plans ( 1 & 3 years)**:
- Commitment to an amount of usage, long workload

**Spot Instances**:
- Short workloads, cheap, can lose instances (less reliable)
- Most cost efficient in AWS
- Useful for workloads that are resilient to failure
	- Batch Jobs
	- Data Analysis
	- Image processing
	- Any distributed workloads
	- Workloads with a flexible start and end time 
- Not suitable for critical jobs or databases 

**Dedicated Hosts**:
- Book an entire physical server, control instance placement
- Purchasing options include:
	- On-demand
	- Reserved
- Useful for software that have complicated licensing model
- Visibility into lower level hardware

**Dedicated Instances**:
- No other customers will share your hardware
![[Pasted image 20241229103015.png]]

**Capacity Reservations**:
- Reserve capacity in a specific AZ for any duration
- No time commitment, no billing discounts
- On-demand rate
- Good for short term, uninterrupted workloads 

#### Summary
---
![[Pasted image 20241229103137.png]]
**Price Comparison**:
![[Pasted image 20241229103208.png]]

#### AWS Charges for IPv4 addresses
---
![[Pasted image 20241229103457.png]]
