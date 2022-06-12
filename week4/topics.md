## Cloud Computing

# what is cloud computing -

somebody else's computer - cloud hosting using a secured network

scaling compute, networking, storage ,and analytics
we are paying for the resources we use.
pay as you go

## Cloud Models

[Public Cloud]
harder to scale up, apps can be quickly provisioned, pay as you go.
owned by cloud services or hosting provider
provides resources and services, accessed via a secured network connection.

[Private Cloud]

a full control self-made orchestration of machines, IT, etc.
organizations create a cloud environment in their data center
the org is responsible for operating the provided services, it does not provide access to outside users
self-owned IT servers, to build a cloud environment.

[Hybrid Cloud]
flexible, orgs determine where to run apps, control security, compliance ,and legal reqs.
combines public and private clouds to allow applications to run in the most appropriate location

## Cloud concepts

high availability | fault tolerance | scalability | elasticity | global reach | customer latency capabilities
agility | predictive cost considerations | disaster recovery | security

[Cloud Computing]

[Scalability]
the ability to add more hardware to support users
a grow in resources to strengthen work

[Elasticity]
adding hardware to prevent bottlenecks in a dynamic manner by auto demand.
dynamic allocation of hardware scale - dynamic scalability matches your workload
scalability in a dynamic scalable manner

[Agility]
the system (for instance Azure) ability to allocate resources to supply-demand - e.g. more power etc.

[Fault Tolerance]
a replicated composition that allows us to do a fail-over into the replication.

fail over mechanism- the system's ability to recover from a loss of its parts
for instance, replicated data center

a dual for the main system - reliable machine - if one falls then the switch redirects users to the secondary machine.
obviously, this costs more- more storage, compute, etc.

[High Availability] -
not a replication but a clone - a way to mitigate the issue- we won't have the same power and capacities but enough to recover - this might have slightly bigger downtime but is cost reduced.
a service that is persistent and

[Disaster Recovery]

a replication of the entire data center
site recovery, fault tolerance - rebuild topology.

[Consumption-based pricing model]
pay for only the resources you use
storage costs also when not in use

## Understand Cloud Service models

[Iaas (Infrastructure as a Service)]

build pay as you go infrastructures by renting servers, vms, storage

[Paas (Platform as a Service)]
reducing the self-service by providing the base configurations- servers, os - leaves the bare bone installations outside
managed services... more into dba it. the platform to run services

[Saas (Software as a Service)]
receive the machine in a ready state no-hassle - users pay for the used software on a subscription model

## Microsoft Azure

[Azure Interfaces (CLI, Portal, Rest API)]
the portal is a ui base where we can control the entire cloud.
CLI - connects to the cloud and operates using the command line.
az vmlist, etc. you can use the cloud shell internally in addition from the portal
rest api - same but using endpoints.

[Regions and Availability Zones]
flexibility and scale, data residency, and the ability to select regions close to users.
region pairs - replicated within a close reach.
zones- as opposed to single vm and less the pairs- provides protection from entire datacenters failures and grants 99.99% sla (the chance of more then 1 virtual machine to fault is low)
fiber optic connected networks and separated datacenter which is physically separated within the same region - provide protection against downtime.

[Resources and Resource Groups]
vms | storage accounts | virtual networks| app services | sql dbs| functions
resource group is a container to manage and aggregate resources in a single unit
resources resides on different regions, can be moved and utilize multiple resource group
its a logical attach - a group of resources

[Essential Compute Services]
[Basic Networking Services]
vnet, ip cidr...

## ]!!![ [Storage Services Fundamentals]

{[ The Azure Storage platform is Microsoft's cloud storage solution for modern data storage scenarios. Azure Storage offers highly available, massively scalable, durable, and secure storage for a variety of data objects in the cloud. ]}
What is the difference between Blob and file storage
{{ Azure Blob Storage is an object store used for storing vast amounts unstructured data, while Azure File Storage is a fully managed distributed file system based on the SMB protocol and looks like a typical hard drive once mounted. }}
Why is it called Blob storage
{{ It allows users to store large amounts of unstructured data on Microsoft's data storage platform. In this case, Blob stands for Binary Large Object, which includes objects such as images and multimedia files.
}}

{{ Azure provides software as a service (SaaS), platform as a service (PaaS) and infrastructure as a service (IaaS). The platform supports many programming languages and frameworks and can be used alone or in a multi-vendor cloud environment. }}

[Understand Database Services]
{{ several of the database services that are available on Microsoft Azure, such as Azure Cosmos DB, Azure SQL Database, Azure SQL Managed Instance, Azure Database for MySQL, and Azure Database for PostgreSQL. In addition, you'll learn about several of the big data and analysis services in Azure }}
...
{{ Azure SQL Database is a fully managed database service, which means that Microsoft operates SQL Server for you, and ensures its availability and performance. SQL Database also includes innovative features to enhance your business continuity, such as built-in high availability.}}
...
{{ Azure offers a choice of fully managed relational, NoSQL and in-memory databases, spanning proprietary and open-source engines, to fit the needs of modern app developers. }}

[Serverless Model Awareness] - example - functions as a standalone serivice
{{ What is serverless computing? Serverless computing enables developers to build applications faster by eliminating the need for them to manage infrastructure. With serverless applications, the cloud service provider automatically provisions, scales and manages the infrastructure required to run the code. }}

{{ Azure Functions is a serverless solution that allows you to write less code, maintain less infrastructure, and save on costs. Instead of worrying about deploying and maintaining servers, the cloud infrastructure provides all the up-to-date resources needed to keep your applications running. }}

## _-_-\*-

extra networking:

4 layer model: tcp/ip:
application layer | transport layer | internet layer | network interface layer
protocols- http/ ftp,pop3 etc. | tcp/udp | ip, arp | ethernet, token ring

7 layer osi model
(app, presentation, session) (physical, data link)
