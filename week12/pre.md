# [Orchestration]
{ What is orchestration in DevOps?
DevOps orchestration is the automation of numerous processes that run concurrently in order to reduce production issues and time to market, 
while automation is the capacity to do a job or a series of procedures to finish an individual task repeatedly. }

[What is Container Orchestration]
{ Container orchestration is the automation of much of the operational effort required to run containerized workloads and services. This includes a wide range of things software teams need to manage a container's lifecycle, including provisioning, deployment, scaling (up and down), networking, load balancing and more. }

[Why do we need Container Orchestration]
{ Container orchestration can be used in any environment where you use containers. It can help you to deploy the same application across different environments without needing to redesign it. And microservices in containers make it easier to orchestrate services, including storage, networking, and security.}
 
[Tools for orchestration (Kubernetes, Docker Swarm, Hashicorp Nomad)]


Docker Swarm is a clustering and scheduling tool for Docker containers. With Swarm, IT administrators and developers can establish and manage a cluster of Docker nodes as a single virtual system. Swarm mode also exists natively for Docker Engine, the layer between the OS and container images.

Nomad is a flexible scheduler and workload orchestrator that enables an organization to easily deploy and manage any containerized or legacy application using a single, unified workflow. Nomad can run a diverse workload of Docker, non-containerized, microservice, and batch applications.


# Kubernetes
{Kubernetes (sometimes referred to as K8s) is an open-source platform that is used to manage and automate the deployment, scheduling, monitoring, maintenance, and operation of application containers across a cluster of machines. Developed by Google, networking with Kubernetes allows administrators to move workloads across private, public, and hybrid cloud infrastructures. Developers use Kubernetes to package software applications with their required infrastructure and deploy new versions quickly.}

[Architecture]

[Yaml & Kubectl]
{kubectl. The Kubernetes command-line tool, kubectl, allows you to run commands against Kubernetes clusters. You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs}
{It is easy to get started with generating YAML files for most of the resources with kubectl. You can use “ — dry-run=client -oyaml > yaml_file. yaml” flag on the “kubectl create” or “kubectl run” commands to generate most of the resources. The file needs to be cleaned a bit, but it is a good starting point.}
{When writing YAML files for Kubernetes, there are four required fields that must be present. APIVersion, Kind, Metadata, and Specifications.}
{using the YAML field allows you to declaratively manage your Kubernetes applications. These YAML files can be stored in a common directory and may all be applied using kubectl apply -f <directory>.}

[Pods]
{ A pod is the smallest execution unit in Kubernetes. A pod encapsulates one or more applications. Pods are ephemeral by nature, if a pod (or the node it executes on) fails, Kubernetes can automatically create a new replica of that pod to continue operations.}

[Deployments & Upgrades]
{A Kubernetes Deployment is used to tell Kubernetes how to create or modify instances of the pods that hold a containerized application. Deployments can scale the number of replica pods, enable rollout of updated code in a controlled manner, or roll back to an earlier deployment version if necessary.}
{Rolling update
The simplest way to update your Kubernetes nodes is to use a rolling update. The is the default upgrade mechanism Kubernetes Engine uses to update your nodes.
A rolling update works in the following way. One by one, a node is drained and cordoned so that there are no more pods running on that node. Then the node is deleted, and a new node is created with the updated Kubernetes version. Once that node is up and running, the next node is updated. This goes on until all nodes are updated.

You can let Kubernetes Engine manage this process for you completely by enabling automatic node upgrades on the node pool.}

[Labels & Annotations]
{ Labels can be used to select objects and to find collections of objects that satisfy certain conditions. In contrast, annotations are not used to identify and select objects. The metadata in an annotation can be small or large, structured or unstructured, and can include characters not permitted by labels.}

[Networking]
https://opensource.com/article/22/6/kubernetes-networking-fundamentals
{Kubernetes networking is designed to ensure that the different entity types within Kubernetes can communicate. The layout of a Kubernetes infrastructure has, by design, a lot of separation. Namespaces, containers, and Pods are meant to keep components distinct from one another, so a highly structured plan for communication is important.}
{ Kubernetes defines a network model that helps provide simplicity and consistency across a range of networking environments and network implementations.}
{ Kubernetes follows an “IP-per-pod” model where each pod get assigned an IP address and all containers in a single pod share the same network namespaces and IP address.}

[Services]
{ A Kubernetes service is a logical abstraction for a deployed group of pods in a cluster (which all perform the same function). Since pods are ephemeral, a service enables a group of pods, which provide specific functions (web services, image processing, etc.) to be assigned a name and unique IP address (clusterIP).}

[Configmaps & Secrets]

{A ConfigMap is an API object that lets you store configuration for other objects to use. Unlike most Kubernetes objects that have a spec , a ConfigMap has data and binaryData fields. These fields accept key-value pairs as their values. Both the data field and the binaryData are optional.}
{If you want to view the binaryData keys (and their values) in a ConfigMap, you can run kubectl get configmap -o jsonpath='{. binaryData}' <name> . Starting with Kubernetes v1. 23, kubectl supports the --from-env-file argument to be specified multiple times to create a ConfigMap from multiple data sources.}

{A Secret is an object that contains a small amount of sensitive data such as a password, a token, or a key. Such information might otherwise be put in a Pod specification or in a container image. Using a Secret means that you don't need to include confidential data in your application code.}
{Both ConfigMaps and secrets store the data the same way, with key/value pairs, but ConfigMaps are meant for plain text data, and secrets are meant for data that you don't want anything or anyone to know about except the application.}
kubectl get secret admin-user-pass -o jsonpath='{.data}'
echo 'amYzOTJoZjc4MmhmOTMyaAo=' | base64 --decode



[Jobs & Cronjobs]

[DaemonSets]
