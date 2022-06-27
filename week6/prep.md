## Configuration Management
{ Configuration management is a systems engineering process for establishing consistency of a product's attributes throughout its life. In the technology world, configuration management is an IT management process that tracks individual configuration items of an IT system.}

# What is Configuration Management
[a config managment is a system of IAC, that allows us to build infrustructure in a reliable, controlled eviroment, above all it is about order and control]
{ Configuration Management is the process of maintaining systems, such as computer hardware and software, in a desired state. Configuration Management (CM) is also a method of ensuring that systems perform in a manner consistent with expectations over time.}

# Why do we need Configuration Management
[ first of all to avoid manual repetetive work on servers, to reduce strain and extend efficency, also cost. both in manual and hands-on efficency comes into mind ]
{ Other benefits of configuration management include: Reduced risk of outages and security breaches through visibility and tracking of the changes to your systems. Cost reduction by having detailed knowledge of all the elements of your configuration, avoiding wasteful duplication of your technology assets.}

# Tools for Configuration management
[ ansible as the leading top notch tech since it is not only open souce but also doesn;t require to install anything on target machines apart from ssh and python above 2.7 (?) .
apart from that we traditionally have Chef, Puppet, i beleive that vagrant as well as jenkins to various parts of deploying assests on a number or even oa fleet of servers .]
{{ Configuration management is a subset of system management. Configuration management tools perform various roles like physical and logical assets. Software Configuration management tools allow you to track the configuration items. }}
{ Ansible is the best configuration management, deployment, orchestration open-source tool and also automation engine. It is a push-based configuration tool. It helps to automate the entire IT infrastructure by providing large productivity gains.}

## Ansible
{{ Red Hat Ansible ... Ansible is an open source community project sponsored by Red Hat, it's the simplest way to automate IT. Ansible is the only automation ..}}
{ Ansible can be used to provision the underlying infrastructure of your environment, virtualized hosts and hypervisors, network devices, and bare metal servers. It can also install services, add compute hosts, and provision resources, services, and applications inside of your cloud. }

# Architecture
{ Ansible is a radically simple IT automation engine that automates cloud provisioning, configuration management, application deployment, intra-service orchestration, and many other IT needs.}
playbook play compose order
# Inventory
{ The Ansible inventory file defines the hosts and groups of hosts upon which commands, modules, and tasks in a playbook operate. The file can be in one of many formats depending on your Ansible environment and plugins. Common formats include INI and YAML. }

# Playbooks
{ An Ansible® Playbook is a blueprint of automation tasks—which are complex IT actions executed with limited or no human involvement. Ansible Playbooks are executed on a set, group, or classification of hosts, which together make up an Ansible inventory.}

# Modules
{ A module is a reusable, standalone script that Ansible runs on your behalf, either locally or remotely. Modules interact with your local machine, an API, or a remote system to perform specific tasks like changing a database password or spinning up a cloud instance. }

# Variables
{ Ansible uses variables to manage differences between systems. With Ansible, you can execute tasks and playbooks on multiple different systems with a single command. To represent the variations among those different systems, you can create variables with standard YAML syntax, including lists and dictionaries.}

# Conditionals
{{ Conditional statements are mostly used in Ansible playbooks where there is a mix of different variables, each representing different entities such as software packages, servers, networking devices and so on.}}
{ If you combine a when statement with a loop, Ansible processes the condition separately for each item. This is by design, so you can execute the task on some items in the loop and skip it on other items.}

# Loops
{ Ansible loop is used to repeat any task or a part of code multiple times in an Ansible-playbook. It includes the creation of multiple users using the user module, installing multiple packages using apt or yum module or changing permissions on several files or folders using the file module.}

# Roles
{ Ansible roles allow you to develop reusable automation components by grouping and encapsulating related automation artifacts, like configuration files, templates, tasks, and handlers. Because roles isolate these components, it's easier to reuse them and share them with other people.}
