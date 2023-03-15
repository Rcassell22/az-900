## Azure Fundamentals

### Cloud Computing

Definition: The delivery of computing services over the internet, or the "cloud".
Some services include:
* Servers
* Storage
* Databases
* Networking
* Software
* Analytics
* Intelligence
* Internet of Things (IoT)
	* basically describes a bunch of different things connecting to the internet. For example, your smart watch, smart TV, smart fridge, smart coffee maker, are all part of the IoT if they can connect to the internet some how.
	
The main benefit of cloud computing is you don't need to increase your phyiscal infrastructure to use any of these services. You pay someone to use the services they're hosting on their infrastructure, which they manage and support themselves.

When you pay for cloud computing services, you're essentially renting the provider's infrastructure and paying for what you use.

#### Basic Cloud Computing Services:
* Compute Power
	* Scalable processing demands.
	* Pay only for the processing resources you use.
* Storage
	* Provides storage that you can access from anything that has access to the cloud.
	* Maintained by someone other than you.

#### Shared Responsibility Model
Definition: When paying a cloud provider for access to their services, both the customer and the provider are responsible for different parts of the service model.
Ex: When paying to store data on the cloud, a provider is responsible for the infrastructure, phyiscal security, power, etc. The customer is responsible for the data and access security (protecting access credentials like login info).

There are some responsibilities that always belong to the provider:
* The physical datacenter
* The physical network
* The physical hosts

Others that belong to the customer:
* The information and data stored in the cloud
* Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
* The accounts and identities of the people, services, and devices within your organization

There are also some responsibilities that fall on one or both parties depending on the service being provided:

**Software as a Service (SaaS)**

| Responsibility | Owner |
| -- | -- |
| Identity and infrastructure | Both |
| Applications | Microsoft |
| Network Controls | Microsoft |
| Operating System | Microsoft |

* Least flexible, but is also the easiest the start up.
* Customer is only really responsible for the data, the users, and devices that access the service.
* Some examples of SaaS are email, financial software, and messaging apps.
	
**Platform as a Service (PaaS)**

| Responsibility | Owner |
| -- | -- |
| Identity and infrastructure | Both |
| Applications | Both |
| Network Controls | Both |
| Operating System | Microsoft |

* Middle ground between IaaS and SaaS.
* Provider maintains the physical infrastructure and security, as well as the OS, middleware, databases, dev tools, and business intel services.
* Example use case would be allowing the customer to create applications with built in software resources.


**Infrastructure as a Service (IaaS)**

| Responsibility | Owner |
| -- | -- |
| Identity and infrastructure | Customer |
| Applications | Customer |
| Network Controls | Customer |
| Operating System | Customer |

* The most flexible cloud service category.
* Gives the customer the most control; they're essentially just renting the hardware to with what they want.
* Provider is responsible for the physical infrastructure and internet connection. The customer has to handle all other maintenance, management, and security tasks.
* An example would be replicating an on-site infrastructure quickly and easily, for development or testing usage. Another wold be migrating from an on-site datacenter to a cloud deployment ("lift and shift").

### Cloud Models

Definition: Cloud models define the deployment type of cloud resources. There are 3 main kinds:

**Private Cloud**
* Used by a single entity.
* Gives the entity/company/IT department more control at a higher monetary cost and fewer benefits of a public cloud deployment.
* Can be hosted in an on-site, off-site, or third-party data center.

**Public Cloud**
* Built, controled, and maintained by a third-party provider.
* Anyone can purchase and access services and resources.

**Hybrid Cloud**
* Uses both public and private clouds.
* Allows private clouds to meet high usage demands by temporarily deploying public cloud resources.
* Provides increased security potential by allowing the user to chose what services they want public or private.

| Public cloud | Private cloud | Hybrid cloud |
| -- | -- | -- |
| No capital expenditures to scale up | Organizations have complete control over resources and security | Provides the most flexibility |
| Applications can be quickly provisioned and deprovisioned | Data is not collocated with other organizations’ data | Organizations determine where to run their applications |
| Organizations pay only for what they use | Hardware must be purchased for startup and maintenance |	Organizations control security, compliance, or legal requirements |
| Organizations don’t have complete control over resources and security |	Organizations are responsible for hardware maintenance and updates | |

**Multi-cloud**
* The "multi" refers to multiple public cloud service providers.
* Might use this model if one provider doesn't have a service you like, but another does, or if you're migrating between providers one service at a time.

**Azure Arc**
Azure Arc is a set of technologies you can use to more easily manage your cloud of environment. It works with any of the cloud models, including multi-cloud.

**Azure VMware Solution**
Azure VMware Solution allows you to run established VMware workloads in Azure with added scalability.

### Consumption-Based Model
Definition: Paying for a resource/service based on how much of it you use.

Two kinds of expenses in IT infrastructure models:
* Capital Expenditure (CapEx):
	* One-time, up-front expenditure for securing tangible resources. Ex: A new building, datacenter, roof repairs, or a company car.
* Operational Expenditure (OpEx):
	* Paying over time for a service. Ex: Renting/leasing, subscription based services.
	* Cloud computing is considered OpEx. You don't pay for the physical infrastructure, just how much of the providers IT resources you use.
	
**Benefits of consumption-based model:**
* No upfront costs.
* No need to manage or purchase infrastructure.
* Ability to utilize more resources when they're needed simply by paying for them.
* Ability to stop paying for resources when they're not being used.

### Benefits of using cloud services
The two biggest benefits of deploying a cloud application are availability and scaling with demand.

**High Availability**
* Azure has uptime guarantees depending on the service.
* High availability ensures maximum availability regardless of disruptions/events/

**Scalability**
* Allows you to add more resources when needed, and only pay for those extra resources when needed thanks to the consumption-based model.
* Vertical Scaling:
	* Adding/Removing RAM and CPUs based on processing power demand.
* Horizontal Scaling:
	* Adding/Removing VMs or containers depending on demand.
	
**Reliability**
* The cloud's decentralized design supports reliable infrastructure.
* If your application is designed properly, the cloud can automatically deploy it to a different region if a catastrophic event occurs in the current deployment.

**Predictability**
* Performance predictability
	* Predicting resources needed to deliver the best experience for your customers.
	* Includes autoscaling, load balancing, and high availability.
* Cost predictability
	* Use cloud analytics to view patterns and trends in your resource usage, and scale it as needed.
	
**Governance** 
* Cloud features like templates make sure all deployed resources meet predefined standards and requirements.
* Easy to update deployments to new standards as they change.
* Auditing features to make sure all resources meet requirements.
* Some software updates and patches are deployed automatically.

**Security**
* Gives the user the option to have complete control over security or let the cloud provider control it.
* Maintenance and patching can be configured to happen automatically.
* Cloud providers are well duited to handle DDoS attacks.

**Manageability**
* Management of the cloud:
	* Automatically scalre resources based on usage.
	* Deploy resource via preconfigured templates.
	* Monitor health, usage, and performance.
	* Automatically replace failing resources.
* Cloud management can be done using APIs, PowerShell/CLI, or a web portal.