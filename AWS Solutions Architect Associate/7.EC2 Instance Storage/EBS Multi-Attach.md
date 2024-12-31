
**Definition**:
EBS Volume attach is only available for io 1/ io 2 family and allows you to attach the same EBS volume to multiple EC2 instances in the same AZ, each instance has full read & write permissions to the high-performance volume

**Use Cases**:
- Used to achieve higher application availability in clustered Linux applications
- Applications must manage concurrent write operations

We can have up to 16 EC2 instances at a time and muse use a file system that is cluster aware