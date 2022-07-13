# Containers

[What are containers]
containers are a sort of precompiled package that can creat images - for instance i can have a container of mysql and run may different images from that container.

{{The key difference between a Docker image vs a container is that a Docker image is a template that defines how a container will be realized. A Docker container is a runtime instance of a Docker image. The purpose of this piece is to answer the question, what is a Docker image vs.}}

[Containers vs VMs]
vm's are a complete machine with it's own hypervisor and os, in a container we can run a minimal, cimpatible mini enviroment to fullfill the exact needs
{ Virtual machines have a host operating system and a guest operating system inside each VM. The guest OS can be any OS, such as Linux or Windows, irrespective of the host OS. In contrast, Docker containers are hosted on a single physical server with the host OS shared among them.}

[Why do we need containers]
{Containers require less system resources than traditional or hardware virtual machine environments because they don't include operating system images. Applications running in containers can be deployed easily to multiple different operating systems and hardware platforms.}
a container is needed to run images, each container will have it's own data pulled from the main docker hub.
{[ Docker streamlines the development lifecycle by allowing developers to work in standardized environments using local containers which provide your applications and services. Containers are great for continuous integration and continuous delivery (CI/CD) workflows.]}

[Docker Commands]
docker run, build, start and stop are just a few commands that can cook up images from containers, there are many more for more advanced usage
{{ docker run – Runs a command in a new container.
docker start – Starts one or more stopped containers
docker stop – Stops one or more running containers
docker build – Builds an image form a Docker file
docker pull – Pulls an image or a repository from a registry
docker push – Pushes an image or a repository to a registry
docker export – Exports a container’s filesystem as a tar archive
docker exec – Runs a command in a run-time container
docker search – Searches the Docker Hub for images
docker attach – Attaches to a running container
docker commit – Creates a new image from a container’s changes }}

[CI/CD for containerized applications]
{ Knowing the benefits of containers, why not put pipelines in them? Containerized pipelines allow for isolation between pipeline jobs. Every single job runs off of a container image which includes all the dependencies needed for that application. Because of this, there aren’t any dependency issues between pipeline jobs – even if they run on the same node! Containers also allow for immutability – once it’s built, it is unchangeable, and if you want to make a change you need to create a new image. Following along with this concept, each pipeline job runtime will be exactly the same. Also with containerized pipelines, the shift to a Kubernetes cluster is easy and allows for scalability. Leveraging Kubernetes as a resource for pipelines is definitely an added benefit.}
{{ Containerized pipelines are software development pipelines where you can define the steps and environments for coding tests, builds, and deploys.}}
i guess it has something to do with the hub and the way we can store containers as artifacts

# Docker

[Architecture]
{ Docker uses a client-server architecture. The Docker client talks to the Docker daemon, which does the heavy lifting of building, running, and distributing your Docker containers. The Docker client and daemon can run on the same system, or you can connect a Docker client to a remote Docker daemon.}
{{Docker follows Client-Server architecture, which includes the three main components that are Docker Client, Docker Host, and Docker Registry.}}
[registery]
A Docker registry is a storage and distribution system for named Docker images. The same image might have multiple different versions, identified by their tags. A Docker registry is organized into Docker repositories , where a repository holds all the versions of a specific image.
[host]
Talking about Docker host, it is the server machine on which Docker daemon runs. Whereas the Docker containers are running instances of Docker images. Docker host can be Bare metal, VM image, iso, image hosted on some clouds etc.
[client]
The Docker client ( docker ) is the primary way that many Docker users interact with Docker. When you use commands such as docker run , the client sends these commands to dockerd , which carries them out. The docker command uses the Docker API. The Docker client can communicate with more than one daemon.
[server]
Docker server is nothing but a compute instance (VM, Personal Computer etc.) which is responsible for runing docker daemon process which in turn manages all the services provided by docker.

layers and binaries, to build images , the docker engine works on the kernel and allows us to use manu containers, os etc.

[Installation]
{{ Install Docker Engine, changing the path below to the path where you downloaded the Docker package. $ sudo dpkg -i /path/to/package.deb. The Docker daemon starts automatically.}}
install docker engine, can now also install docker desktop on ubuntu, on win it can use wsl or hypervisor to function

[CLI]
{When running the command, the Docker CLI client checks the value the variable has in your local environment and passes it to the container.}

has many functions, rich variety of commands, can start, stop, pull push containers and images.

[Dockerfiles]
{A Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image. Using docker build users can create an automated build that executes several command-line instructions in succession. This page describes the commands you can use in a Dockerfile .}
a special king of precederual files for instance - sing FROM - gets to pull the image from the hub, from which the container would be built.
dockerfiles can structure the image, transfer files and build and prepare for the run.

[Registries]
{ A Docker registry is a storage and distribution system for named Docker images. The same image might have multiple different versions, identified by their tags. A Docker registry is organized into Docker repositories , where a repository holds all the versions of a specific image.}
repo connected?
repositories containing the dockerfile and souce code etc.

[Volumes]
{ Docker volumes are file systems mounted on Docker containers to preserve data generated by the running container. The volumes are stored on the host, independent of the container life cycle. This allows users to back up data and share file systems between containers easily}
volumes are saved states of the containes, they are shared, you can keep one and load it into another or several machines.

[Networking]
{ Docker networking allows you to attach a container to as many networks as you like. You can also attach an already running container. Go ahead and attach your running web app to the my_bridge . $ docker network connect my_bridge web. Open a shell into the db application again and try the ping command.}
apart from portsm containers "talk to each other" over the "bridge"

[Debugging]
{If you are having trouble with Docker containers or images, you can enable debug mode on your Docker daemon. Enabling debugging provides more verbose output from the daemon and you can use this information to find out more about why your containers or images are having issues.}
{ Debugging a failed docker build. Checking the content of the application and its build inside the docker container. Checking the logs of the application. Installing something inside the container at runtime in order to test something.}

[Docker Compose]
{ Docker Compose is a tool that was developed to help define and share multi-container applications. With Compose, we can create a YAML file to define the services and with a single command, can spin everything up or tear it all down.}
yaml file that can orchestrate several containers.
and also manage dependencies between them.
