## Final work closing the Linux Administration Course 2021
   __________________________________________________________

### Topic: Linux Privilege Escalation
______________________________________

#### Introduction

> Privilege escalation is the act of exploiting a flaw in an operating system or in a software application to gain elevated access to protected ressources in order to perform unauthorized actions. One of the main role of a system administrator is to prevent these exploits but the weakest link in a system still remains the human part, a badly administered user with the wrong privileges and permissions could lead a company to a disaster. 
In this study, we will see how a poorly administered user can be abused and how this could enable a malicious person to obtain full privileges.



#### Methodology 

> Assume that the rogue organization or the white hat hired to test your security has already the control over the targeted user, we will not approach the preliminary  vulnerabilities research to access to the shell although some of the same methods will be used to scan for any vulnerabilities from the compromised user's terminal.
> Everybody has his own practice to manage his entry point from the shell but there is a process no one escapes, the enumeration. This enumeration consists in collecting any datas that could lead to a breach to exploit, specific files will be automatically scrutinized, to that end, the intruder will use self-made or existing tools.

#### Targets:

We will explore basic examples of Linux privilege escalation. There are more advanced exploits that involve more attack vectors like exploiting softwares at the source but this is not the point of the topic. In our presentation, we will detail three attacks:

- The Kernel, we will use a VM with Ubuntu 16.04 LTS and its vulnerable kernel (4.4.0-116).

- Cron jobs, we will use a VM with Debian 11 and a wrongly privileged crontab.

- And how History file could compromise your security with another VM with Debian 11.


