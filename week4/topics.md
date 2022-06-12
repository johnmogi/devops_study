## Cloud Computing

https://www.youtube.com/watch?v=urc2A-05PyE&list=PLBkJ88wLiM-g_N1nBpmzVf0xAx-h8MDOm&index=12

https://bootcamp.rhinops.io/week-04/overview/slides/

# what is cloud computing -

somebody else's computer - cloud hosting using a secured network

scaling compute, networking, storage and analytics
we are paying for the resources we use.
pay as you go

## Cloud Models

[Public Cloud]
harder to scale up, apps can be quickly provisioned, oay as you go.
owned by cloud services or hosting provider
provides resources and services, accessed via secured network connection.

[Private Cloud]

a full control self made orchestration of machines, IT etc.
organizations create a cloud enviroment in their data center
the org is responsible for operating the provided services, it does not provide access to outside users
self owned it servers, to build a cloud environment.

[Hybrid Cloud]
flexible, orgs determine where to run apps, control security, compliance and legal reqs.
combines public and private clouds to allow applications to run in the most appropriate location

## Cloud concepts

high availability | fault tolerance | scalability | elasticity | global reach | customer latency capablities
agility | predictive cost considerations | disaster recovery | security

[Cloud Computing]

[Scalability]
the ability to add more hardware to support users
a grow in resources to strenghten work

[Elasticity]
adding hardware to prevent bottlenecks in a dynamic manner by auto demand.
dynamic allocation of hardware scale - dynamic scalability matches your worload
scalability in a dynamic scalable manner

[Agility]
the system (for instance Azure) ability to alocate resources to supply demand - e.g. more power etc.

[Fault Tolerance]
a replicated composition that allows us to do a fail over into the replication.

fail over mechanism- the system's ability to recover from a loss of it's parts
for instance replicated data center
a dual for main system - reliable machine - if one falls then the switch redirects users to the secondary machine.
obviously this costs more- more storage, compute etc.

[High Availability] -
not a replication but a clone - a way to metigate the issue- we won't have the same power and capacities but enough to recover - this might have slightly bigger downtime but is cost reduced.
a service that is persistent and

[Disaster Recovery]

a replication of the entire data center
site recovery, fault tolerance - rebuild topology.

[Consumption based pricing model]
pay for only the resources you use
storage costs also when not in use

## Understand Cloud Service models

[Iaas (Infrastructure as a Service)]

build pay as you go infrastructures by renting servers, vms, storage

[Paas (Platform as a Service)]
reducing the self service by providing the base configurations- servers, os - leaves the bare boe installations outside
managed services... morre into dba the it. the platform to run services

[Saas (Software as a Service)]
recive the machine in a ready state no hassle - users pay for the used software on a subscription model

## Microsoft Azure

[Azure Interfaces (CLI, Portal, Rest API)]
the portal is a ui based where we can control the entire cloud.
CLI - connects to the cloud and operates using the command line.
az vmlist, etc. you can use the cloud shell internally in addition from the portal
rest api - same but using endpoints.

[Regions and Availability Zones]
flexability and scale, data residency, the ability to select regions close to users.
region pairs - replicated within a close reach.
zones- as opposed to single vm and less the pairs- provides protection from entire datacenters failures and grants 99.99% sla (the chance of more then 1 virtual machine to fault is low)
fiber optic connected networks and seperated datacenter wich are phisically seperated within the same region - provides protection against downtime.

[Resources and Resource Groups]
vms | storage accounts | virtual networks| app services | sql dbs| functions
resource group is a container to manage and aggregate resources in a single unit
resources resides on different regions, can be moved and utilize multiple resource group
its a logical attach - a group of resources

[Essential Compute Services]
[Basic Networking Services]
vnet, ip cidr...

## ]!!![ [Storage Services Fundamentals]

[Understand Database Services]
[Serverless Model Awareness]

## _-_-\*-

extra networking:

4 layer model: tcp/ip:
application layer | transport layer | internet layer | network interface layer
protocols- http/ ftp,pop3 etc. | tcp/udp | ip, arp | ethernet, token ring

7 layer osi model
(app, presentation, session) (physical, data link)
