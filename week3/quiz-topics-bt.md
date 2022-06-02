before training - bt

Development [8]
{{ the process of conceiving, specifying, designing, programming, documenting, testing, and bug fixing involved in creating and maintaining applications, frameworks, or other software components.}}

Web Servers [8]
{{ A web server is computer ; The hardware used to run a web server can vary according to the volume of requests that it needs to handle. At the low end of the ...  }}

Compilation [7]
{{ Compilation is the process the computer takes to convert a high-level programming language into a machine language that the computer can understand. The software which performs this conversion is called a compiler. High-level language, Machine language, Programming terms }}

Binary Files [6]
{{ A binary file is a computer file that is not a text file. The term "binary file" is often used as a term meaning "non-text file". Many binary file formats ... }}

Build Artifacts [6]
{ Build artifacts are files produced by a build. Typically, these include distribution packages, WAR files, reports, log files, and so on. When creating a build configuration, you specify the paths to the artifacts of your build on the Configuring General Settings page }

Package Management [7]
{{ Package management is the process of handling the many and varied dependencies and artifacts for your servers, applications, and developers. These are the archives, binaries, libraries, tools, scripts, modules, snippets, metadata, assets and even datasets that power your processes, products, and solutions. }}

Universal Repository Management [7]
{{ The task of managing access to all the public repositories and components used by your development teams can be simplified and accelerated with a dedicated server application known as a 'repository manager'. A repository manager provides the ability to proxy remote repositories and cache and host components locally. }}

Operations [7]
{{ Operations is the work of managing the inner workings of your business so it runs as efficiently as possible. Whether you make products, sell products, or provide services, every small business owner has to oversee the design and management of behind-the-scenes work. }}

Linux Fundamentals [8]
{{ Linux allows a user to control every aspect of the operating system. As Linux is an open-source operating system, it allows a user to modify its source (even source code of applications) itself as per the user requirements. Linux allows the user to install only the desired software nothing else (no bloatware). }}

Linux Package Management [7]
{{ Package management is a method of installing, updating, removing, and keeping track of software updates from specific repositories (repos) in the Linux system. Linux distros often use different package management tools }}
DPKG | apt-get | yum | snap etc.

Working with Files and Directories [9]
{{ Linux stores data and programs in files. These are organized in directories. In a simple way, a directory is just a file that contains other files (or directories). The part of the hard disk where you are authorised to save data is calle your home directory. }}
mkdir | touch | chmod | cat | mv | cp | rm | cd

Linux Essential Commands [8]
rmdir | locate | find | grep | sudo | df | du | tail head | diff | tar
jobs | kill | chown | ping | wget | uname | top | history | man | echo |
useradd | userdel |

Text Editors in Linux [8]
nano | vi | vim

Environment Variables [7]
{{ In Linux and Unix based systems environment variables are a set of dynamic named values, stored within the system that are used by applications launched in shells or subshells. In simple words, an environment variable is a variable with a name and an associated value.

printenv

set

MY_VAR='Linuxize'

/etc/environment - Use this file to set up system-wide environment variables. Variables in this file are set in the following format:

To load the new environment variables into the current shell session use the source command:

source ~/.bashrc
}}

Networking in a Nutshell [5]

{{ What is a network? Well, a network is nothing more than a collection of connected devices and end points and end systems with the purposes of exchanging and sharing information.

Now, today the network is a collection of devices and end systems, but those end systems include almost anything, not only computers, servers, but also telephones and cell phones and industry-automation machines that will now be involved in the exchange of information. That means we are exchanging not only data or traditional data in the form of files and other components, but also voice and video and multimedia collaboration.
}}

sela lecture:
computers comuniacate using ip's
ip is composed of 4 digits wit 3 dots.
each block of 3 numbers represents a class (a,b,c) - with allowed ip range.
each class represents 0-255 (256 numbers)
a lot of addresses are limited or reserved - that's why ipv4 is slowly running out of available ips.
there are additional private routes reserved for networks for instance routers.

12.0.0.1/8
mask
127.255.255.255

result 3 mistakes:

Summary

avatar
jonathan Moguillansky
Assignment

Accuracy
85%
Score
16370
Performance Stats
17
Correct
3
Incorrect
12 s
Time/ques
Review Questions
Click on the questions to see answers

3.  Which of the following is not an operating system?
    Windows 10

Linux -V

GNU/Linux

Solaris -X

10. An application was deployed and is available at port 8081, you try to connect but get connection refused, what could be the reason?
    The Firewall doesn't allow traffic into the port -V

Port 8081 is not a valid port

The application port-tool is not installed

All options are correct - X

20. What project is Linux based on?
    DOS

Unix - X

GNU -V

Minix

1.  How do you connect to a terminal in a remote Linux server?
    Using SSH

Using RDP

Using HTTP

Using HTTPS

2.  Which of the following best defines what a network is
    Computers with internet access

Computers linked to provide a storage service

A group of computers connected to a printer

Group of computers connected for the exchange of data

4.  Which of the following is not a text editor?
    Nano

Vim

Notepad

Screen

5.  What is the name of the systems that know how to store various types of packages?
    Universal Repository Manager

Hybrid Repository Manager

Cloud Package Manager

ArtifactsHub

6.  What is the process used to convert the code into binary files?
    Package Management

Compilation

Debugging

Interpretation

7.  Which of these options is not a Linux distro?
    Ubuntu

Fedora

Linux Server 2019

CentOs

8.  What protocol is used when users need to transmit sensitive data, such as logging into a bank account, email service, or health insurance provider
    FTP

HTTP

HTTPS

HTML

9.  What is apt?
    A Monitoring Tool

A Package management tool for Windows

A Network Protocol

A Package management tool for Linux

11. What is the root user?
    There is no such thing

User that by default has access to all commands and files

User that by default has access to certain commands and files

User that by default has access to no commands and files

12. Nuget is the package manager for:
    Java

Python

C#

Nodejs

13. Every machine on a network needs a unique IP address?
    True

False

14. How do you move a file or directory in Linux?
    move /path/to/file /new/path/to/file

mv /path/to/file /new/path/to/file

move-file /path/to/file /new/path/to/file

Move-Item /path/to/file /new/path/to/file

15. How do you access a remote Windows server Desktop?
    Using SSH

Using RDP

Using HTTP

Using HTTPS

16. Binary files are human-readable?
    True

False

17. What is the native Windows web server?
    IIS

Ngnix

Apache

Jetty

18. What's the name of the Linux pet?
    Laika

Tux

Moby

Gopher

19. A load balancer...
    Create a secure tunnel through an insecure network

Distribute the load among multiple endpoints

Expose the applications to the internet

All the answers are correct
