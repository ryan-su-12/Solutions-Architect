When you create an Encrypted EBS volume:
- Data at rest is encrypted inside the volume
- All the data in flight moving between the instance and the volume is encrypted 
- All snapshots are encrypted
- All volumes created from the snapshot
Encryption and decryption are handled transparently (you have nothing to do)
Its good to do this because encryption has a minimal impact on latency, and copying an unencrypted snapshot allows encryption 

**Encrypt an unencrypted EBS volume**:
- Create an EBS snapshot of the volume
- Encrypt the EBS snapshot
- Create new EBS volume from the snapshot
- Now you can attach the encrypted volume to the original instance