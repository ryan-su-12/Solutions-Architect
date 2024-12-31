#### 2 sorts of IPs
---
- IPv4: 1.160.10.240
- IPv6: 3ffe: 1900:4545:3:200:f8ff:fe21:67cf

**Public IP**:
- Public IP means the machine can be identified on the internet
- Must be unique across the whole web
- Can be geo-located easily
![[Pasted image 20241229142817.png]]
**Private IP:**
- Private IP means the machine can only be identified on a private network only
- The IP must be unique across the private network
- Two different private networks can have the same IPs
- Machines connect to WWW using NAT + internet gateway (a proxy)
- Only a specified range of IPs can be private IPS
![[Pasted image 20241229142826.png]]

**Elastic IPs**:
- When you stop and then start an EC2 instance, it can change its public IP
- If you need to have a fixed public IP for you instance, you need an elastic IP
- An elastic IP is a public IPV4 IP you own as long as you don't delete it 
- You can attach it to one instance at a time
- With an elastic IP address, you can mask the failure of an instance or software by rapidly remapping the address to another instance in your account
- Important for applications that require consistent IP addresses

Note that we use a load balancer and don't use a public IP
![[Pasted image 20241229142835.png]]

![[Pasted image 20241229142504.png]]
![[Pasted image 20241229142848.png]]
