# Module 3

## Use Google Cloud to build your Apps 

### Objectives
1. Explore the role of compute options in the cloud
2. Learn about building and managing virtual machines
3. Examine building elastic applications using autoscaling
4. Explore PaaS options by leveraging App Engine
5. Examine building event-driven services using Cloud Run functions
6. Identify containerizing and orchestrating applications with Google Kubernetes Engine
7. Identify developing and deploying scalable containerized applications with Cloud Run

-----------------------------------------------------------------------------------------------------------------------------

## Compute Options
![Cloud Services](https://i.imgur.com/BgCy3IW.png)


#### Compute Options
- Good for general work

#### PaaS
- Use App Engine

#### Cloud Run Functions
- Serverless option to run code based on some sort of event (bot idea?)

-----------------------------------------------------------------------------------------------------------------------------

## Exploring IaaS with Compute Engine

With Compute Engine, users can create and run virtual machines on Googles virtual datacenters and networks.
A virtual machine can run like an operating system and be configured to any of your needs. 
You can run any computing workload such as web hosting, application hosting, or backend stuff.

You can create a virtual machine using the Google cloud console. 

##### Peremptible CPUs
- Can help save you 90% on VM & vCPU costs for workloads that does not require a human to sit there and inspect it.
- You can use Google cloud online price calculator to check how much your task can cost

-----------------------------------------------------------------------------------------------------------------------------

## Exploring PaaS with App Engine

Basically, go with App engine if you just want to write code and not actually touch or work with Cloud infrastructure. Its a quick way to scale your application quickly. App engine allows you to have high availability apps without complex architecture. 

##### How does it work?

![How does it work](https://i.imgur.com/FjnibnF.png)

App Engine also provides Software Development kits (SDKs)
- API and libraries
- Sandbox environment
- Deployment tools

#### Now, there are two types of App Engine environments:
The App Engine Standard Environment
- Has persistent storage with queries, sorting, and transactions
- Automatic scaling and load balancing
- Asynchronous task queues for performing work outside the scope of a request
- Scheduled tasks for triggering events at specified times or regular intervals
- Integration with other Google Cloud services

There are however two requirements to run the standard environment: 
1. Use specified versions of Java, Python, PhP, GO, Node.js, and Ruby
2. Applications must conform to sandbox restraints

## The Standard Environment Workflow

![Workflow](https://i.imgur.com/qej3zhZ.png)

-------------------------------------------------------------------------------------------------------------------------------

## Then we get into the flexible environment
- Instances are health-checked, healed, and co-located
- Critical backwards-compatible backups are automatically made and applied to the system
- VM instances are automatically located by geographical regions according to the settings in your project
- VM instances are restarted on a weekly basis

#### Advantages of flexible environments
1. Take advantage of custom configurations and libraries, while focusing on writing code
2. Customize the runtime and the operating system of your VM
3. Customize or provide runtimes by supplying a custom Docker image or Dockerfile

### Lets Compare the two Environments:

![Compare](https://i.imgur.com/89R2FM4.png)

---------------------------------------------------------------------------------------------------------------------------------

## Containerization (Kubernetes)

The Google Kubernetes Engine is a mix of the Compute Engine (with servers, networking, storage) and the App Engine (Present run-times, managed services).

![Table](https://i.imgur.com/ysqLCZ3.png)

#### Now what is a Container?
Think of it like an invisible box around your code and its dependencies. It has limited access to its own partition of the file system and hardware. Only requires a few system calls to create and starts working ASAP. You need an OS kernel that supports containers and a container runtime, on each host. It scales like [PaaS](https://github.com/Sarkis-Gaf/Notes-Google-Cloud-Fundamentals/edit/main/Intro%20Module%203.md#exploring-iaas-with-compute-engine) but has the same flexibility as IaaS.

You probably want build your application with multiple containers, each performing its own function. You can make them modular and easily deployable. 

### What is Kubernetes?

![Kubernetes](https://i.imgur.com/xsJc69R.png)

GKE (Google Kubernetes Engine) is a managed environment for deploying containerized apps. It is a sophisticated management system that runs docker containers in the google cloud. Think of it like a container organizer. 
















