# Computing technology that makes Cloud Computing possible

This chapters explains the fundamentals of servers and datacenters inclduing software development.
This is the core fundament of why cloud providers like AWS exist.

---

## 1. Servers and Datacenters

### Servers
Servers are powerful computers that provide resources and services to other computers. 
Provides a response to a request from a client computer over a network.
- has more memory and multiple CPUs
- reside in data centers

Examples:
- Web server
- Database server
- Mail server

### Datacenters
A physical localtion to host computer systems and their technical components.
- Power supply
- Cooling systems
- Security measures
- Network connectivity

### On Premise vs. Cloud Model
On-premise:
- Host at your own location
- Manage and finance all the hardware and software, including maintenance staff

Cloud model:
- Service provider owns and provides hardware and infrastructure
- You pay to use the providers resources and services

**AWS relevance:**
AWS operates massive datacenters filled with servers to provide cloud services globally.

---

## 2. Virtual machines
Software emulation of a physical computer
- Runs on a physical computer called host
- Runs its own OS
- Hypervisor provides access the hosts physical components
- Virtualization enables multiple VMs on a single physical machine

Running VMs reduces cost, increases utilization, reusability and portability with a single physical machine.
That makes them a fundamental unit of computing in the cloud.

**AWS relevance:**
EC2 instances are virtual machines running on AWS's physical servers.
You only pay for the capacity that you use and cam quickly scale capacity if computing requirements change.

---

## 3. SDLC - Software development life cycle
A process for planning, creating, testing, and deploying software applications.
It's iterative and repeats over time.

Phases:

1. Plan (Project Plan): 
    - Define the problem and how to solve.

2. Analyze (Software Requirements Sepcification): 
    - What do you want from a solution?

3. Design (Design Specification document): 
    - How to built.

4. Develop (Coding):
    - Build the design.

5. Test (Unit testing etc.): 
    - Expected output fulfilled?

6. Implement (Deployment to prod):
    - Use what you built.

7. Maintain (Monitoring and maintenance): 
    - Improve built.


**AWS relevance:**
AWS provides tools and services to support each phase of the SDLC, such as:

    AWS CodeCommit (source control)
    AWS CodeBuild (build service)
    AWS CodeDeploy (deployment service)
    AWS CodePipeline (CI/CD service)
    AWS Cloud9 (cloud-based IDE)
    AWS Lambda (serverless compute for running code without provisioning servers)
    AWS CloudFormation (infrastructure as code for managing resources)
    AWS CloudWatch (monitoring and logging)
    AWS Elastic Beanstalk (platform as a service for deploying applications)
    AWS CloudTrail (audit and compliance)
