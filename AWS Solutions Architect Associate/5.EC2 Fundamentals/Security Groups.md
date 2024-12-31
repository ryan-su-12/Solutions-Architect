Security Groups are fundamental of network security in AWS
- They control how traffic is allowed into or out of our EC2 instances
- Security groups only contain allow rules
- Security group rules can reference by IP or by security group 
- Act as a firewall
![[Pasted image 20241227173556.png]]
Security groups regulate:
- Access to ports
- Authorized IP ranges - IPv4 and IPV6
- Control of inbound network
- Control of outbound network 
![[Pasted image 20241227173714.png]]
**Security Group Diagram**:
![[Pasted image 20241227173852.png]]
**Good to know**:
- Can be attached to multiple instances
- Locked down to a region/VPC combination
- Lives "outside" the EC2 instance, if the traffic is blocked the EC2 instance won't see it
- It's good to maintain one separate security group for SSH access
- If your application is not accessible, then it's a security group issue
- If your application gives a "connection refused" error, then it's a application error or it's not launched
- All inbound traffic is blocked by default
- All outbound traffic is authorized by default 

**Classic Ports to know**:
- 22 = SSH (secure shell) - log into a Linux instance
- 21 = FTP (File transfer protocol) - upload files into a file share
- 22 = SFTP ( Secure file transfer protocol) - upload files using SSH
- 80 = HTTP - access unsecured websites
- 443 = HTTPS - access secured websites 
- 3389 = RDP (remote desktop protocol) - log into a windows instance 