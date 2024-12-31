EBS volume are network drives with good but "limited" performance
So if we need a high-performance hardware disk, use EC2 Instance Store
Its used for:
- Better I/O performance
- But EC2 instance store lose their storage if they're stopped
- Good for Buffer/ Cache/ Scratch data/ temporary content
- Also risk of data loss if hardware fails
- Backups and replication are the users responsibility