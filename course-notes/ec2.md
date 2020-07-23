- Launching virtual machines (EC2)
- Storing data on virtual drives (EBS)
- Distributing load across machine (ELB)
- Scaling services using auto scaling groups (ASG)
- Subnet = AZ
- key pair, gives access to login to ec2
- Avoid using Elastic IP, use random public and register a DNS
  - or load balancer

### Ec2 User Data

- **Bootstrapping** launching commands when the machine starts
- automate boot straps
  - install updates
  - install software
  - download common files
- Runs with root user

### Instance Launch Types

- On Demand: short workload, create - get it right away
  - predictable pricing - pay exactly for what you use (per second)
  - Highest cost - no long term commitment
    - Good for short term work
- Reserved (min 1 year) - up to 3 years
  - Good for **database**
  - Can get up to 75% discount - pay upfront
  - reserved instances - long workloads
  - **convertable**, can convert size in middle of year
  - **scheduled reserved** - every thursday 3 to 6pm
    - if you have a process you run then
- Spot instance - short workload, super cheap, can lose instances (less reliable)
  - up to 90% discount
  - batch job
  - data analyst
  - image process
  - retry
- Dedicated instances - no customers share hardware
  - Running on hardware dedicated to you
  - Can share hardware with other instances, but ONLY in the same account
- Dedicated Host - book **entire** physical server
  - *sockets, cores, host ID*
  - Physical dedicated - full control of placement
  - 3 year period reservation
  - Bring Your Own License
  - Companies with strong compliance
- **Great combo** - Reserve for baseline + Spot/On Demand during peaks