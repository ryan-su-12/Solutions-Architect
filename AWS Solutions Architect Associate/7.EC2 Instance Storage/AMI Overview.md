![[Pasted image 20241230111007.png]]

Amazon machine image
- AMI = Amazon Machine Image
- AMI are a customization of an EC2 instance
	- You add your own software, configuration, operating system, monitoring
	- Faster boot / configuration time because all your software is pre-packaged
- AMI are built for a specific region
So far we have been using Public AMI to launch our EC2 instances, we can also create our own AMI and then also use an AMI someone else made on the AWS marketplace 

**AMI Process**:
1. Start an EC2 instance and customize it
2. Stop the instance (for data integrity)
3. Build an AMI - Will create an EBS snapshot
4. Launch instances from other AMIs
![[Pasted image 20241230105924.png]]
