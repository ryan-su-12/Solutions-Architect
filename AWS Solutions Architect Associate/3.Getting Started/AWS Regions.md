Many regions around the world obviously, but in terms of AWS a region is a cluster of data centers. Most AWS services are region-scoped

**Possible Question: How to choose an AWS region**:

If you need to launch a new application, where should you do it, well it depends. 
- Compliance: You need to be compliant with data governance and legal requirements: data never leaves a region without your explicit permission 
- Proximity to customer: Reduced latency 
- Available Services: New services and new features aren't always available in every region 
- Pricing: pricing varies region to region and is transparent in the service pricing page

**AWS Availability Zones**:

Each region can have many availability zones (min is 3, max is 6)
- So lets say we have the AWS region Sydney: ap-southeast-2
	- ap-southeast-2a
	- ap-southeast-2b
	- ap-southeast-2c
	each of these availability zones is one or more discrete data centers with redundant power, networking, and connectivity. They are separate from each other, so that they are isolated from disasters. They're connected with high bandwidth, ultra-low latency networking
	

**AWS Points of Presence (Edge Locations)**:
- Amazon has 400+ Points of Presence in 90+ cities across 40+ countries
	- 400 + Edge locations 
	- 10 + regional caches
- Content is delivered to end users with lower latency 