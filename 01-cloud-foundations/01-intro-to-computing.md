This chapter explains the fundamentals of how computers work. 
In AWS, every EC2 instance, container, and serverless runtime is built on these same concepts.

1. Hardware vs. Software
A computer always consists of:

• Hardware (physical components)
◇ CPU – computes
◇ Memory (RAM) – temporary working space
◇ Storage – persistent data
◇ Network card – communication

• Software
◇ Operating System (OS) – controls everything
◇ Applications – what actually runs


AWS relevance:
◇ An EC2 instance is a virtual computer with virtual CPU, RAM, disk, and network.
◇ Setting up you choose:
▪ vCPU & RAM - Instance type (e.g., t3.micro)
▪ Storage - EBS (SSD/HDD)
▪ OS - Amazon Linux, Windows, etc.



2. CPU – Compute Power
◇ Executes instructions from OS and applications
◇ Has cores → more cores = more parallel work = higher performance


AWS relevance:
◇ Instance types differ mainly in:
▪ Number of vCPUs
▪ Performance class
◇ More CPU = better for compute-heavy workloads (e.g., processing, encryption, analytics)



3. Memory (RAM)
◇ Holds active programs and data
◇ Temporary – lost when powered off
◇ Measured in MB/GB
◇ More RAM = smoother and faster execution


AWS relevance:
◇ RAM is fixed per instance type
◇ Too little RAM = slow apps, crashes
◇ Memory-heavy apps (databases, caches) require RAM-optimized instances



4. Storage Drives
◇ Persistent – data retains after shutdown
◇ Types:
▪ HDD – cheaper, slower
▪ SSD – faster, more expensive

◇ Performance measured in:
▪ MB/s
▪ IOPS (Input/Output Operations per Second)


AWS relevance:
◇ Maps directly to Amazon EBS
▪ gp3, io2 = SSD (fast)
▪ st1, sc1 = HDD (cheap, slow)

◇ Choose storage based on:
▪ Performance needs
▪ Cost



5. Networking
◇ Connects computers to share data
◇ Wired or wireless
◇ The internet is the largest network


AWS relevance:
◇ Every EC2 instance has:
▪ A virtual network interface (ENI - Elastic Networtk Interface)
▪ An IP address


◇ Communication happens inside:
▪ VPCs
▪ Subnets
▪ Security Groups
◇ Cloud is network-first architecture



6. Network Interface Card (NIC)
◇ Enables network communication
◇ Measured in Gbps


AWS relevance:
◇ EC2 network performance depends on:
▪ Instance type
▪ ENI capabilities
◇ High-throughput workloads need high network bandwidth



7. Operating System (OS)
◇ Manages CPU, memory, storage, and network
◇ Provides CLI or GUI
◇ Examples:
▪ Windows, macOS, Linux (in AWS especially Amazon Linux 2)


AWS relevance:
◇ You must choose an OS when launching EC2
◇ OS determines:
▪ Available tools
▪ Package management
▪ Security updates
◇ Amazon Linux is optimized for AWS


Summary:
“An EC2 instance is just a computer with CPU, RAM, storage, and network – virtualized and managed by AWS.”
◇ CPU = compute
◇ RAM = temporary working memory
◇ Storage = persistent data
◇ Network = communication
◇ OS = resource manager