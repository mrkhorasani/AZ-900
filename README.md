# AZ-900
**FedRAMP**: The **Federal Risk and Authorization Management Program** is a United States federal government-wide compliance program that provides a standardized approach to security assessment, authorization, and continuous monitoring for cloud products and services.

**CapEx:** **Capital expenditure** or **capital expense** is the money an organization or corporate entity spends to buy its fixed assets, such as servers, buildings, vehicles, equipment, or land.

**OpEx:** **Operational expenditure** is the money an organization or corporate entity spends to maintain, or improve its fixed assets, such as hitting ventilation, electricity, human and manpower, and payroll costs.

**NIST**: National Institute of Standards and Technology https://csrc.nist.gov/publications/detail/sp/800-145/final

**Cloud computing** is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources that can be rapidly provisioned and released with minimal management effort or service provider interaction. 

**Federal Chief Information Officer of the United States says,** There was a time when every household, town, farm, or village had its water well. Today, shared public utilities give us access to clean water by simply turning on the tap; cloud computing works similarly. Just like water from the tap in your kitchen, cloud computing services can be turned on or off quickly as needed. Like at the water company, there is a team of dedicated professionals making sure the service provided is safe, secure, and available on a 24/7 basis. When the tap isn't on, not only are you saving water, but also you aren't paying for resources you don't currently need.
https://www.brookings.edu/wp-content/uploads/2012/04/0407_cloud_computing_kundra_remarks.pdf

Virtual Machine Vs Container Vs Serverless-Computing
![image](https://github.com/mrkhorasani/AZ-900/assets/51242725/b21dbcaa-b007-4590-8c49-8bd9a403b62e)
> [!Note]  
> In the cloud, you have to pay for VMs and Containers idle times, but you only pay for the cost of Serverless-Computing runtime.
When you have an error in an application, you need to troubleshoot only the function that made a mistake for you separately, not all of the application. So this troubleshooting method doesn't affect all aspects of your application.
--------------------------------------------------------------------------------------------------------
## **Benefits of Cloud:**

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
--------------------------------------------------------------------------------------------------------
## **Cloud Types:**<br>
   1. Public Cloud
   2. Private Cloud<br>
      is common among companies that have to avoid data disclosure to the public. military services and companies that have to comply with HIPPA.
   3. Hybrid Cloud
> [!Note]
> **HIPAA:** Stands for "Health Insurance Portability and Accountability Act" which defines standards to prevent patient data from being disclosed to the public.<br>
> **Multi-Tenancy:**  Cost-saving by sharing computing resources with other cloud users.
--------------------------------------------------------------------------------------------------------
## **Cloud Main Services Category:**<be>
![image](https://github.com/mrkhorasani/AZ-900/assets/51242725/ed0d94c4-efc1-475a-b26b-1e47c9c4e53c)
##IaaS: 
Stands for Infrastructure As A Service<br>
**Common use cases of IaaS:**
   1. Migrating Workload
   2. Test and Dev
   3. Website Hosting
   4. Backup, Storage and Recovery
## PaaS:
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
   4.  Big Data: We have a built cluster under this category. it's more like a warehouse, which just needs to specify its parameters such as "Size and Type" to get it up and running quickly. We have an interface to interact with this platform on certain tools to monitor the help. Monitoring and Patching is also the vendor's responsibility. Some examples of Big  Data services are Azure Data Lake, Microsoft HDInsight, Amazon REDSHIFT, AWS EMR"Elastic MapReduce", and Google's Big Table.
## SaaS:
Stands for "Software As A Service" is a method of software delivery, usually with an annual or monthly subscription fee
