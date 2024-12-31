- Possible to get a discount of up to 90% compared to on-demand
- Define max spot price and get the instance while current spot price < max
	- Hourly spot prices varies on offer and capacity
	- You have a 2 minute grace period where you can stop or terminate your instance
- Spot block
	- You block a spot instance during a specified timer frame without interruptions

You can only cancel spot instance requests that are open, active, or disabled
Cancelling a spot request does not terminate instances. You must firs cancel a spot request, and then terminate the associated spot instances

**Spot Fleets**:
- Spot fleets = set of spot instances + (optional) On-Demand Instances
- Spot fleet will try to meet the target capacity with price constraints 
	- Defines possible launch pools: instance type (m5.large), OS, Availability Zone
	- Can have multiple launch pools, so that the fleet can choose
	- Spot fleets stop launch instances when reaching capacity or max cost 
**Strategies to allocate spot instances**:
- Lowest Price: from the pool with the lowest price (cost optimization, short workload)
- diversified: distributed across all pools (great for availability, long workloads )
- Capacity Optimized: pool with optimal capacity for the number of instances
- priceCapcaityOptimized: pool with highest capacity available, then select the pool with the lowest price (best choice for most workloads)
Spot fleets allow us to automatically request spot instances with the lowest price

