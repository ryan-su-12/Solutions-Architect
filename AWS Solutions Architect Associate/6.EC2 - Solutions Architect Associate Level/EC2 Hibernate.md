**EC2 Hibernate** is a feature in Amazon EC2 that allows you to **pause** your instance and **resume it later** while retaining the instance's state, including memory (RAM) contents, disk contents, and processes. It’s like putting your laptop into sleep mode rather than shutting it down completely.
Use cases include, long running processing, saving the RAM sate and services that take time to initialize 

**Good to know**:
- Supported instance families - C3, C4 C5, I3, M3, M4, R3, R4, T2, T2, ..
- Instance RAM size - must be less than 150 GB
- Instance Size - note supported for bare metal instances
- Available for On-demand, reserved, and spot instances
- An instance can not be hibernated more than 60 days 