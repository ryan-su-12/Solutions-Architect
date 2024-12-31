- Make a backup of your EBS volume at a point in time
- Not necessary to detach volume to do snapshot
- can copy snapshots across AZ or region
![[Pasted image 20241230105016.png]]
#### EBS Snapshot Features
---
**EBS Snapshot Archive**:
- Move a snapshot to an "archive tier" that is 75% cheaper
- Takes within 24 to 72 hours to restore the archive
**Recycle bin for EBS Snapshot**:
- Setup rules to retain deleted snapshots so you can recover them after an accidental deletion
- Specify retention 

**Fast Snapshot Restore**:
- Force full initialization of snapshot to have no latency on the first use