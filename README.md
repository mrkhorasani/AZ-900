# AZ-900
**FedRAMP**: The **Federal Risk and Authorization Management Program** is a United States federal government-wide compliance program that provides a standardized approach to security assessment, authorization, and continuous monitoring for cloud products and services.

**CapEx:** **Capital expenditure** or **capital expense** is the money an organization or corporate entity spends to buy its fixed assets, such as servers, buildings, vehicles, equipment, or land.

**OpEx:** **Operational expenditure** is the money an organization or corporate entity spends to maintain, or improve its fixed assets, such as hitting ventilation, electricity, human and manpower, and payroll costs.

**NIST**: National Institute of Standards and Technology https://csrc.nist.gov/publications/detail/sp/800-145/final

**Cloud computing** is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources that can be rapidly provisioned and released with minimal management effort or service provider interaction. 

**Federal Chief Information Officer of the United States says,** There was a time when every household, town, farm, or village had its water well. Today, shared public utilities give us access to clean water by simply turning on the tap; cloud computing works similarly. Just like turning on water from your kitchen tap, cloud computing services can be quickly activated or deactivated as needed. Like at the water company, there is a team of dedicated professionals making sure the service provided is safe, secure, and available on a 24/7 basis. When the tap isn't on, not only are you saving water, but also you aren't paying for resources you don't currently need.
https://www.brookings.edu/wp-content/uploads/2012/04/0407_cloud_computing_kundra_remarks.pdf

Virtual Machine Vs Container Vs Serverless-Computing
![image](https://github.com/mrkhorasani/AZ-900/assets/51242725/b21dbcaa-b007-4590-8c49-8bd9a403b62e)
> [!Note]  
> In the cloud, you have to pay for VMs and Containers idle times, but you only pay for the cost of Serverless-Computing runtime.
When you have an error in an application, you need to troubleshoot only the function that made a mistake for you separately, not all of the application. So this troubleshooting method doesn't affect all aspects of your application.
## Benefits of Cloud
1. Cost Effective
   It does not need much upfront cost and, has a Predictive cost consideration capability
2. Scalability <br>
   2.1 Vertical Scaling: like an increase of RAM in the spike in traffic (Scale Up) <br>
   2.2 Horizontal Scaling: like auto-adding a WebServer in the spike in traffic load (Scale Out)
   ![image](https://github.com/mrkhorasani/AZ-900/assets/51242725/6ff3da70-70e4-41c0-a590-1f758d74a046)
3. Elasticity<br>
   Dynamically increase or decrease the resources as needed 
4. Current/Updated<br>
   Hardware and software updates, the latest patches will be installed by CSP(Cloud Service Provider)
5. Reliable<br>
   Disaster Recovery Plan, Redundancy, Fault Tolerance(to be up and running), Backup by CSP
6. Cloud is Global(Global Reach)<br>
   Cloud services are located in different regions (Available Zone), for the best response time. Cloud users can replicate their services into multiple regions for redundancy and the least latency.
7. Security<br>
   7.1 Physical: Guards, walls, cameras, gates, security personnel, and .etc...<br>
   7.2  Digital & Cyber: firewalls and security software and tools
8. Agility<br>
   Allocate or de-allocate resources quickly
## Cloud Types
   1. Public Cloud
   2. Private Cloud<br>
      is common among companies that have to avoid data disclosure to the public. Military services and companies that have to comply with **HIPPA**.
   3. Hybrid Cloud
> [!Note]
> **HIPAA:** Stands for "Health Insurance Portability and Accountability Act" which defines standards to prevent patient data from being disclosed to the public.<br>
> **Multi-Tenancy:**  Cost-saving by sharing computing resources with other cloud users.
----------------------------------------------------------------------------
## Cloud Main Services Category
![image](https://github.com/mrkhorasani/AZ-900/assets/51242725/ed0d94c4-efc1-475a-b26b-1e47c9c4e53c)
## IaaS 
Stands for Infrastructure As A Service<br>
**Common use cases of IaaS:**
   1. Migrating Workload
   2. Test and Dev
   3. Website Hosting
   4. Backup, Storage and Recovery
## PaaS
Stands for "Platform As A Service" sometimes referred to as **Serverless Design or Architecture** is a platform for our application, it's anything you may need for your application such as Database, Web Server, etc. By PaaS, you don't need to worry about your OS, monitoring, patching, antiviruses, backup, and other underlying structures like hardware.<br>
**Common use cases of PaaS:**
   1. DBMS: DataBase Management Service (Such As Azure SQL or Amazon RDS"Relational Database")
         1.1. manage by the cloud provider<br>
         1.2. Support and backup by CSP<br>
         1.3. Has its monitoring system to optimize database configuration and optimizes by CSP<br>
   2. Web Application Hosting Service: A runtime application (like Azure Webapps, Elastic Bean Stalk, and GAE) for your web application like PHP, JAVA, NodeJS, .NET, and .etc<br>
         2.1. There is built-in application monitoring
         2.2. Error logging
         2.3. No runtime management (Patching is done automatically)
   3.  Container Orchestrator(like Azure container services which coupled with docker, Amazon Elastic container services and google container engine and google Kubernetes engine)
   4.  Big Data: We have a built cluster under this category. It's more like a warehouse, which just needs to specify related parameters such as "Size and Type" to get it up and running quickly. We have an interface to interact with this platform on certain tools to monitor the help. Monitoring and Patching is also the vendor's responsibility. Some examples of Big  Data services are Azure Data Lake, Microsoft HDInsight, Amazon REDSHIFT, AWS EMR"Elastic MapReduce", and Google's Big Table.
## SaaS(Software as a Service)
This is a method of software delivery typically with an annual or monthly subscription fee, like Office 365, Gmail, Salesforce CRM, etc.
## Azure Regions
Microsoft Azure data centers are located around the world, these data centers are organized and made available to end users by region. Each region is a geographical area on the planet containing at least one, but potentially multiple data centers. 
Azure has more global regions than any other cloud provider as of today.
Azure is available in 42 regions worldwide, with more than 12 additional regions planned and announced.
### Azure Special Region
These special regions are specifically for the U.S government agency and partners that are screened by U.S persons and include compliance certifications, and located in the following areas:
   1. U.S DOD (Department of Defense)
      1.1. Central
      1.2. Virginia
      1.3. IOWA
These are isolated physical and logical from Azure. 
   2. CHINA: Microsoft Azure operated by 21Vianet (Azure in China) is a physically separated instance of cloud services located in China
      2.1. East
      2.2. North
   3. GERMANY: T-Systems(Dutch telecom company) manages this area of azure
      3.1. Central
      3.2. North-East
### Reginal Paired
Each data center in every region is coupled and synced with another in the same area to implement redundancy and replicate cloud resources such as VMs, Storage, etc. This issue aims to  implement zero downtime service in the case of natural disasters, power outages, physical network outages, civil unrest, etc. 
This link shows the list of paired regions https://learn.microsoft.com/en-us/azure/reliability/cross-region-replication-azure
### Feature Availability
It means that not all Azure services are available in all regions. Some services like Active Directory, DNS, and Traffic Manager are global, while others are hosted in dedicated regions.
## Availability Zone
AZ are separated locations within a region. Each AZ is made up of one or more data centers that are equipped with independent power, cooling, and network. It is designed to have an isolated boundary. There are three separate AZs in all enable regions. 
![image](https://github.com/mrkhorasani/AZ-900/assets/51242725/972643a4-f6d0-485c-b05d-86259f765b76)
## Availability Sets
This is a way to ensure our application and services remain online and aren't affected by software and hardware updates and maintenance time. To keep online services during the update of software and hardware in these data centers done through two mechanisms:
   1. Update Domain: Servers in an update domain perform updates sequentially. An update domain consists of all servers where an application is installed in order of redundancy, and servers reside on separate racks. Upgrading processes such as installing patches, firmware, and BIOS on these servers are done sequentially to ensure app and service outages do not affect end-users' service accessibility.
   2. Fault Domain
