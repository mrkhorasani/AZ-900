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
## SaaS
Software as a Service is a method of software delivery. Typically, with an annual or monthly subscription fee, like Office 365, Gmail, Salesforce CRM, etc.
## Azure Regions
Microsoft Azure data centers are situated worldwide and are organized by region to provide access to end users. Each region is a geographical area on the planet that houses at least one, but potentially multiple data centers.
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
   ### 1. Update Domain
   Servers in an update domain perform updates sequentially. An update domain consists of all servers where an application is installed in order of redundancy, and servers reside on separate racks. Upgrading processes such as installing patches, firmware, and BIOS on these servers are done sequentially to ensure app and service outages do not affect end-users' service accessibility.
   ### 2. Fault Domain
This one provides physical separation of workloads across different hardware in the data centers. It means that we have several racks with separated power supply, cooling, and network connection paths that consist of multiple servers, so in the case of hardware upgrades or maintenance, services(apps) are always accessible and available because services and apps reside on several physical servers across the multiple rack or fault domain.

## Resource Group
**Definition:** A resource group is a logical container for Azure resources, which include virtual machines, databases, storage accounts, and more.
**Purpose:** It allows for the management and organization of resources in a structured way. You can deploy, update, and delete all the resources in a resource group together.<br>
**Management Scope:** Resources in a resource group share the same lifecycle. You can apply management and access control policies, such as role-based access control (RBAC), to the resource group.<br>

### Key Features of Resource Groups
1. **Organizational Unit**:<br>
It helps organize resources logically, making managing and maintaining them easier.
2. **Lifecycle Management**:<br>
Resources in the same resource group can be managed, deployed, and deleted together. This makes resource groups an efficient way to handle the lifecycle of multiple resources.
3. **Access Control**:<br>
You can apply access control policies to the entire resource group. This means you can grant permissions to users or groups at the resource group level, which then applies to all resources within the group.
4. **Dependency Management**:<br>
Helps in managing dependencies between resources during deployment. For example, you can ensure a database is created before the web application depends on it.
5. **Monitoring and Billing**:<br>
You can view and manage costs and monitor the health and performance of resources within a resource group collectively.

> [!Note]
> By organizing resources into resource groups, Azure users can manage their cloud resources more effectively, ensuring that related resources are managed as a cohesive unit. This organizational structure simplifies management tasks and enhances the overall efficiency of resource management in Azure.
> 
Connecting to Azure Resource Manager (ARM):
You can use various tools and interfaces. Here are the common methods to connect to and interact with Azure Resource Manager:

1. Azure Portal
The Azure Portal is a web-based interface that allows you to manage your Azure resources visually.

Steps to Connect:
Navigate to the Azure Portal.
Sign in with your Azure account credentials.
Once logged in, you can manage your resources using the graphical user interface.
2. Azure CLI
Azure CLI (Command-Line Interface) is a cross-platform command-line tool for managing Azure resources.

Steps to Connect:
Install Azure CLI from this link.
Open your terminal or command prompt.
Log in to your Azure account using the command:
bash
Copy code
az login
Follow the instructions to complete the authentication process.
Once logged in, you can use various az commands to manage your resources. For example:
bash
Copy code
az group create --name MyResourceGroup --location eastus
3. Azure PowerShell
Azure PowerShell is a set of modules that provide cmdlets to manage Azure resources directly from PowerShell.

Steps to Connect:
Install Azure PowerShell by following the instructions here.
Open PowerShell.
Log in to your Azure account using the command:
powershell
Copy code
Connect-AzAccount
Follow the instructions to complete the authentication process.
Once logged in, you can use various Azure PowerShell cmdlets to manage your resources. For example:
powershell
Copy code
New-AzResourceGroup -Name MyResourceGroup -Location eastus
4. REST API
Azure Resource Manager also provides REST APIs for programmatic access to Azure services.

Steps to Connect:
Obtain an access token by authenticating with Azure AD. This can be done using tools like curl, Postman, or any HTTP client library in your preferred programming language.
bash
Copy code
curl -X POST -H "Content-Type: application/x-www-form-urlencoded" -d "grant_type=client_credentials&client_id=<YOUR_CLIENT_ID>&client_secret=<YOUR_CLIENT_SECRET>&resource=https://management.azure.com/" https://login.microsoftonline.com/<YOUR_TENANT_ID>/oauth2/token
Use the access token to make authenticated requests to the Azure Resource Manager REST API. For example, to list resource groups:
bash
Copy code
curl -X GET -H "Authorization: Bearer <ACCESS_TOKEN>" -H "Content-Type: application/json" https://management.azure.com/subscriptions/<SUBSCRIPTION_ID>/resourcegroups?api-version=2021-04-01
5. Azure SDKs
Azure SDKs provide libraries for various programming languages like .NET, Java, Python, JavaScript, etc., to interact with Azure services.

Steps to Connect:
Install the Azure SDK for your preferred programming language. For example, for Python:
bash
Copy code
pip install azure-mgmt-resource
Use the SDK to authenticate and interact with Azure Resource Manager. Example in Python:
python
Copy code
from azure.identity import DefaultAzureCredential
from azure.mgmt.resource import ResourceManagementClient

credential = DefaultAzureCredential()
subscription_id = 'YOUR_SUBSCRIPTION_ID'
resource_client = ResourceManagementClient(credential, subscription_id)

# List all resource groups
for rg in resource_client.resource_groups.list():
    print(rg.name)
These methods allow you to connect to Azure Resource Manager and manage your Azure resources effectively. Choose the one that best fits your workflow and preferences.
