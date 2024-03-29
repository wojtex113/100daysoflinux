Hi all,

My name's Wojtek and I own business called 'WOJST Usługi Informatyczne Wojciech Stańczyk' with a website https://wojst.pl<br/>
I write my thoughts, tips and another IT notes on the blog, which can be found at https://wojst.pl/blog

Today (29-04-2023) I've started the #100DaysOfLinux challenge. My goal is to finish all courses I have purchased but haven't yet completed and complete many labs during this time.

**Update:**
Today (06-08-2023) I've finished this challenge :)

I aspire to be a Linux Administrator, which is my main goal, and I'm also considering the possibility of working in DevOps or SysOps.

Additionaly, I'm a firefighter in Państwowa Straż Pożarna, where we work 24-hour shifts every three days. During my shifts I will try found a few minutes to read or watch something related to this challenge.

So, let's get started :)

--<br/>
var ASL = course 'Administracja Serwerami Linux' by Grupa ADM<br/>
var ADL = course 'Akademia Debugowania Linuksa' by Jakub ‘unknow’ Mrugalski <br/>
var Proxmox Lab = https://wojst.pl/webhosting-lab-w-oparciu-o-proxmox/

---

### :yellow_circle: Day 1 (Saturday, 29-04-2023)
**Git**
- work with git (create remote repo and push commits)<br/>
https://wojst.pl/github-repozytoria-zdalne-i-pull-requesty-git/<br/><br/>
**ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - user management**
- exercises about users management in Linux (performed on Ubuntu running in Docker)<br/><br/>

### :yellow_circle: Day 2 (Sunday, 30-04-2023) [Firefighter duty]
**Docker**
- watch a film on YT from IT conference - "how Docker work inside"

### :yellow_circle: Day 3 (Monday, 01-05-2023)
**ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - file management**
- exercises about file management in Linux (performed on Ubuntu running in Docker)

### :yellow_circle: Day 4 (Thuesday, 02-05-2023)
**ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - Apache**
- configure the web server (Apache), which is running on Ubuntu as a virtual machine in VirtualBox 

### :yellow_circle: Day 5 (Wednesday, 03-05-2023)
- read news and articles about Linux

### :yellow_circle: Day 6 (Thursday, 04-05-2023)
**NGINX**
- "nginx in a hour" course by Jakub ‘unknow’ Mrugalski - I used virtual machine with Red Hat as the lab system

### :yellow_circle: Day 7 (Friday, 05-05-2023)
**ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - Nginx**
- configure the web server (NGINX), which is running on Red Hat as a virtual machine in VirtualBox 

### :yellow_circle: Day 8 (Saturday, 06-05-2023) [Firefighter duty]
**ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - Nginx**
- I'm finishing yesterday's nginx excercises

### :yellow_circle: Day 9 (Sunday, 07-05-2023)
- listen podcasts about Linux

### :yellow_circle: Day 10 (Monday, 08-05-2023)
**Ansible**
- "Ansible in a hour" course by Jakub ‘unknow’ Mrugalski (6 lessons out of 9)<br/>
run 3 Ubuntu virtual machines in VirtualBox and manage them with Ansible from a VM with Red Hat

### :yellow_circle: Day 11 (Thuesday, 09-05-2023) [Firefighter duty]
- read articles on redhat.com

### :yellow_circle: Day 12 (Wednesday, 10-05-2023)
**Ansible**
- "Ansible in a hour" course by Jakub ‘unknow’ Mrugalski (other lessons)<br/>
- ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - Ansible<br/>
run 5 Ubuntu virtual machines in VirtualBox and manage them with Ansible from a VM with Red Hat<br/><br/>
- create blog post titled "How did my adventure with Linux start?"<br />
https://wojst.pl/jak-zaczela-sie-moja-przygoda-z-linuxem/<br/>

### :yellow_circle: Day 13 (Thursday, 11-05-2023)
**Ansible**
- continued ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - Ansible

### :yellow_circle: Day 14 (Friday, 12-05-2023) [Firefighter duty]
- read news about Linux

### :yellow_circle: Day 15 (Saturday, 13-05-2023)
**Ansible**
- continued ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski - Ansible

### :yellow_circle: Day 16 (Sunday, 14-05-2023)
- watch a film on YT from IT conference - "Vagrant a nauczanie informatyki"

### :yellow_circle: Day 17 (Monday, 15-05-2023)
**Ansible**
- I finished the 'Ansible' section in the ebook '77 zadań dla adminów'. I used ChatGTP during this lab.<br/><br/>
All answers added to blog post:<br/>
https://wojst.pl/ebook-77-zadan-dla-adminow-odpowiedzi/<br/><br/>

**OpenVPN [ASL] + pfSense**<br/>
I installed an OpenVPN server on Red Hat host and an OpenVPN client on RHEL as well. Next, I added 2 pfSense VMs beetwen the VPN hosts. All VMs ran in VirtualBox. I configured an internal network between the 'LAN networks'. On pfSense I configured port forwarding to forward a port from the WAN to the LAN OpenVPN server. Below is a schema of the lab.<br /><br/>

![Schema: OpenVPN + pfSense](openvpn_pfsense-schema.png)<br/>

**Docker**<br/>
I did 6 (from 11) excercises from the 'Docker' section in the ebook '77 zadań dla adminów' late in the evening.

### :yellow_circle: Day 18 (Thuesday, 16-05-2023)
**Docker**<br/>
Finished 'Docker' section in the ebook.<br/><br/>

**Routing [ASL]**<br/>
I configured an RHEL VM as a router for another VMs in VirtualBox. Below is the schema of the lab.<br/><br/>

![Schema: RHEL router](routing_rhel_router.jpg)<br/>

Post on the blog:<br/>
https://wojst.pl/linux-jako-router-na-podstawie-rhel/<br/>

### :yellow_circle: Day 19 (Wednesday, 17-05-2023)
**Disk management [ASL]**<br/>
Red Hat lab in VirtualBox: add disk to VM, create / remove partition (fdisk), mount created partition (mount, umount, lsblk, /etc/fstab), LVM management.<br />
It wasn't covered in the course, but I wanted to relab RAID (from Red Hat's official documentation): add 2 disks to a VM, create RAID1, simulate failed disk (remove second disk from VM), add new disk and attempting to repair the RAID.

**Proxmox - install and add to jFrog**<br/>
I intend to create a project with a lot of VMs (HA with KeepAlived, nginx + 2 versions of PHP as a web serwer, Redis to storing sessions, NFS for storing web files, MariaDB servers with replication, pfsense as gateway to this subnet, monitoring, FTP to upload web files etc).<br/>
For this purpose, I have installed Proxmox on an personal computer. To have access from flat I connected it to jFrog. In the next step I installed Debian and Rocky Linux in VMs, which were then converted to templates. I also installed pfSense in a VM and created an internal network.

### :yellow_circle: Day 20 (Thursday, 18-05-2023)
**Proxmox Lab**<br/>
Created and configured 2 VMs (from templates) for MariaDB servers with replications: master using RockyLinux, slave using Debian.<br/><br/>
On the blog I created a post in which I describe the progress of work on the project. This post will be updated as work progresses.<br/>
https://wojst.pl/webhosting-lab-w-oparciu-o-proxmox/

### :yellow_circle: Day 21 (Friday, 19-05-2023)
**[ASL]**<br/>
- management of services (systemctl, create own service)<br/>
- syslogs

**Proxmox Lab**<br/>
Created a NFS server to store web files (based on RockyLinux). In addition, I added two disks that I connected with RAID (mirroring) to this VM. On them I will store the data made available by NFS.

### :yellow_circle: Day 22 (Saturday, 20-05-2023)
**[ASL]**<br/>
Management logs with journalctl.

### :yellow_circle: Day 23 (Sunday, 21-05-2023) [Firefighter duty]
- watch a film on YT: "DevOps - kim jest i czym się zajmuje?"

### :yellow_circle: Day 24 (Monday, 22-05-2023) 
**Samba [ASL]**<br/>
Samba server installation and configuration, creating new shares.<br/><br/>
Outside of the course, I set up Samba as a domain controller with roaming profiles.

### :yellow_circle: Day 25 (Thuesday, 23-05-2023) 
**SELinux [ASL]**<br/>
An introdution to SELinux.<br/><br/>

**Proxmox Lab**<br/>
I installed nginx on two VMs (Debian and RockyLinux) and mounted NFS share to /var/www/html on both servers. On pfSense, I forwarded SSH ports to manage all servers from the outside.

### :yellow_circle: Day 26 (Wednesday, 24-05-2023) [Firefighter duty]
**Proxmox Lab**<br/>
I installed two versions of php (7.4 and 8.1) as fpm on both web servers. Additionaly, I created NFS share with vhost configurations and mount as RO on web servers.

### :yellow_circle: Day 27 (Thursday, 25-05-2023) 
**Proxmox Lab**<br/>
Installation and configuration of SFTP serwer (proftpd).<br/>
I have installed proftpd and disabled access for anonymous. Additionaly, I have added local users (as homedir directory from NFS mounted share, shell false). The servers has been configured to work as SFTP only. I have modified the configuration to allow only users from the ftp_users group (to which I added both users).

### :yellow_circle: Day 28 (Friday, 26-05-2023) 
**Hardening systemd [ASL]**<br/><br/>
**Proxmox Lab**<br/>
Adding a service in which a Python script works to change the owner of new files uploaded via FTP. I explained this in a blog post.

### :yellow_circle: Day 29 (Saturday, 27-05-2023) [Firefighter duty]
**ProxySQL**<br/>
Theoretical introduction to the ProxySQL

### :yellow_circle: Day 30 (Sunday, 28-05-2023) 
**ProxySQL**<br/>
I watched on YouTube films about 'how ProxySQL works'.

### :yellow_circle: Day 31 (Monday, 29-05-2023) 
**Proxmox Lab**<br/>
I installed ProxySQL on a VM with Debian and added both database servers to it. Next, I uploaded files from the backup of my main webpage via FTP, restored the database from a copy and started cloning of wojst.pl. I also had to install php-mysqli.

### :yellow_circle: Day 32 (Thuesday, 30-05-2023) [Firefighter duty]
**Security + backup [ASL]**<br/>
This module contains penetration tests (with Kali Linux) and creating backup with rsync.

### :yellow_circle: Day 33 (Wednesday, 31-05-2023) 
**Troubleshooting [ASL]**<br/>
Introduction to troubleshooting.<br/><br/>

**Proxmox Lab**<br/>
Started installation HAProxy with keepalived on two VMs (Debian+Rocky).

### :yellow_circle: Day 34 (Thursday, 01-06-2023) 
**Proxmox Lab**<br/>
I did troubleshoot yesterday's implementation of HAProxy - I typed incorect IP addresses of web servers.<br/><br/>

**Troubleshooting + bash scripts [ASL]**<br/>
Continuation of troubleshooting - monitoring. Next, there was an introduction to scripting with bash (only as a reminder).<br/><br/>

### :yellow_circle: Day 35 (Friday, 02-06-2023) [Firefighter duty]
**Prometheus + Grafana**<br/>
I watched a video on YT about infrastructure monitoring using Prometheus and grafana.

### :yellow_circle: Day 36 (Saturday, 03-06-2023)
Video on YT: Ciekawe podejście do integracji technologii chmurowych - Piotr Pyciński

### :yellow_circle: Day 37 (Sunday, 04-06-2023)
Read news and articles about Linux.

### :yellow_circle: Day 38 (Monday, 05-06-2023) [Firefighter duty]
**Rsyslog [ASL]**<br/>
Install and configure log server.

### :yellow_circle: Day 39 (Thuesday, 06-06-2023) 
**Troubleshooting [ASL]**<br/>
- test hard disk and memory<br/>
- DRP<br/>
- How to troubleshoot Linux problems (using the example of zabbix_agent)?

### :yellow_circle: Day 40 (Wednesday, 07-06-2023) 
**Troubleshooting [ASL]**<br/>
In th 10th module's homework I troubleshooted problems on a VM with CentOS - IP configuration, SSH service and Apache.

### :yellow_circle: Day 41 (Thursday, 08-06-2023) 
**Bash scripting [ASL]**<br/>
Variables in bash scripts.<br/><br/>

Review of articles and news.

### :yellow_circle: Day 42 (Friday, 09-06-2023) 
**Automatization [ASL]**<br/>
- loop IF, functions in bash script<br/>
- introdution to Ansible <br/><br/>

I wrote an e-book about bash scripting in 2020: https://wojst.pl/wp-content/uploads/2023/01/BONUS-bash_podstawy.pdf

### :yellow_circle: Day 43 (Saturday, 10-06-2023) 
Today I finished a course **"Administracja Serwerami Linux"** by Grupa ADM.<br/><br/>

**Strace [ADL]**<br/>
Introduction to the application's diagnostics with strace.

### :yellow_circle: Day 44 (Sunday, 11-06-2023) [Firefighter duty]
Review of the job interviewer's questions.

### :yellow_circle: Day 45 (Monday, 12-06-2023)
**Strace [ADL]**<br/>
Debugging nginx and apache2 with strace.

### :yellow_circle: Day 46 (Thuesday, 13-06-2023)
**[ADL]**<br/>
Debugging cron and Docker.<br/><br/>

**Proxmox Lab**<br/>
On Proxmox CT, I installed Docker and created container inside it with phpMyAdmin (which is linked to ProxySQL). Next, on the web servers, I added a proxy pass from the domain/phpmyadmin to the container.

### :yellow_circle: Day 47 (Wednesday, 14-06-2023)
Repair of a WordPress-based website - virus removal, access restoration and finally protection.

### :yellow_circle: Day 48 (Thursday, 15-06-2023)
Video on YT about web UI for Ansible.

### :yellow_circle: Day 49 (Friday, 16-06-2023)
Running a web UI for Ansible as a Docker container - as seen in yesterday's video.

### :yellow_circle: Day 50 (Saturday, 17-06-2023) [Firefighter duty]
Configuration an Ansible Semaphore.

### :yellow_circle: Day 51 (Sunday, 18-06-2023)
I watched videos on YT about working as a sysadmin and about Cloudflare.

### :yellow_circle: Day 52 (Monday, 19-06-2023)
**[ADL]**<br/>
A review of the process content in the /proc directory and an introduction to the 'Out of memory killer' mechanism.

**Lab**<br/>
- Create a local environment in VirtualBox to test Ansible's playbooks before committing it to the repo.
- Create an Ansible playbook for the installation and configuration unattended updates on all VMs.

### :yellow_circle: Day 53 (Thuesday, 20-06-2023)
**[ADL]**<br/>
- debugging a bash scripts,<br/>
- compile and install programs from source,<br/>
- recovery mysqld root password<br/><br/>

**Proxmox Lab**<br/>
Create an Ansible playbook for the installation and configuration fail2ban - blocks sshd.

### :yellow_circle: Day 54 (Wednesday, 21-06-2023)
**[ADL]**<br/>
Apache performance tuning - configurate MPM.

### :yellow_circle: Day 55 (Thursday, 22-06-2023)
**[ADL]**<br/>
- problems with ssh connections<br/>
- problems with disk space<br/><br/>

**Proxmox Lab**<br/>
I installed Redis on VM with RockyLinux.

### :yellow_circle: Day 56 (Friday, 23-06-2023) [Firefighter duty]
Video on YT: Linux Interview Questions nad Answers

### :yellow_circle: Day 57 (Saturday, 24-06-2023)
Review news about Linux - It's FOSS news.

### :yellow_circle: Day 58 (Sunday, 25-06-2023)
Overview of ideas for lab projects

### :yellow_circle: Day 59 (Monday, 26-06-2023) [Firefighter duty]
**[ADL]**<br/>
Disk management: copy the partition layout on second disk

### :yellow_circle: Day 60 (Thuesday, 27-06-2023)
**Proxmox Lab**<br/>
- reconfigure backups of VMs (keep the last one, delete the backup 'clean_os'),<br/>
- add Redis VM to an Ansible Semaphore,<br/>
- install and configure Redis WordPress plugin

### :yellow_circle: Day 61 (Wednesday, 28-06-2023)
**Proxmox Lab**<br/>
I've created an Ansible playbook that set up a website environment (including database, user, vhost configuration, etc.)

### :yellow_circle: Day 62 (Thursday, 29-06-2023)
**Proxmox Lab**<br/>
- resolve the problem with the mysql.user table on mariadb-slave<br/>
- improve yesterday's Ansible playbook<br/><br/>

**[ADL]**<br/>
- debugging problems with inodes on disks<br/>
- recovering deleted data

### :yellow_circle: Day 63 (Friday, 30-06-2023)
**[ADL]**<br/>
An Introduction to Uncomplicated Firewall (UFW).

### :yellow_circle: Day 64 (Saturday, 01-07-2023)
Review of articles and news.

### :yellow_circle: Day 65 (Sunday, 02-07-2023)
View video on YT about Kasm Workspaces. 

### :yellow_circle: Day 66 (Monday, 03-07-2023)
**[ADL]**<br/>
- How work with disk backup in the file?
- additional files attributes

### :yellow_circle: Day 67 (Thuesday, 04-07-2023)
**[ADL]**<br/>
- disk load check
- working with a lot of files<br/><br/>

**Docker**<br/>
I've create an environment to practice ProxySQL: 2 containers of MariaDB with replication, 2 containers of phpMyAdmin (to manage data in dbs) and a container with ProxySQL.<br/><br/>

**VPS**<br/>
I created a bash script to clean backups (removing all files older than 20 days).

### :yellow_circle: Day 68 (Wednesday, 05-07-2023) [Firefighter duty]
Video on YT: Poczta w dzisiejszych czasach i podejście w stylu "devops" (SysOps / DevOps Polska)

### :yellow_circle: Day 69 (Thursday, 06-07-2023)
**[ADL]**<br/>
Working with RAID arrays and LVM.

### :yellow_circle: Day 70 (Friday, 07-07-2023)
**[ADL]**<br/>
- How to troubleshoot network issues?<br/>
- debugging DNS problems

### :yellow_circle: Day 71 (Saturday, 08-07-2023) [Firefighter duty]
Watch the film about HA on YT.

### :yellow_circle: Day 72 (Sunday, 09-07-2023)
Watch the film about awesome Linux terminal tools on YouTube.

### :yellow_circle: Day 73 (Monday, 10-07-2023)
**[ADL]**<br/>
- working with routing<br/>
- ssl certs

### :yellow_circle: Day 74 (Thuesday, 11-07-2023) [Firefighter duty]
Prometheus & Grafana - video tutorial on YT.

### :yellow_circle: Day 75 (Wednesday, 12-07-2023) 
**Proxmox Lab**<br/>
I've installed monitoring using Prometheus & Grafana.

### :yellow_circle: Day 76 (Thursday, 13-07-2023) 
**Proxmox Lab - Prometheus & Grafana**<br/>
- installed the Node Exporter on the monitoring VM<br/>
- added it to the Prometheus targets<br/>
- imported the dashboard 'Node Exporter Full'<br/>
- created Ansible playbook which install the Node Exporter on servers

### :yellow_circle: Day 77 (Friday, 14-07-2023) 
**Proxmox Lab**<br/>
- created Docker container with dnsmasq<br/>
- added targets (with hostnames) to Prometheus<br/><br/>

**[ADL]**<br/>
Accessing Linux with a forgotten root password.

### :yellow_circle: Day 78 (Saturday, 15-07-2023) 
**[ADL]**<br/>
Usefull apps - HTOP, XARGS.

### :yellow_circle: Day 79 (Sunday, 16-07-2023) 
Review of articles and news.

### :yellow_circle: Day 80 (Monday, 17-07-2023) 
**[ADL]**<br/>
- SSH tunneling
- troubleshooting email issues
- nethogs

### :yellow_circle: Day 81 (Thuesday, 18-07-2023) 
**[ADL]**<br/>
- Usefull apps - netcat, iptraf-ng<br/>
- Extending SWAP space<br/>
- Gather server information<br/>
- Backup of a full disk to another host

### :yellow_circle: Day 82 (Wednesday, 19-07-2023) 
**[ADL]**<br/>
I've troubleshooted and repaired "zjebanos" (by Jakub ‘unknow’ Mrugalski).<br/><br/>

Today I finished a course **"Akademia Debugowania Linuksa"** by Jakub ‘unknow’ Mrugalski.<br/><br/>

### :yellow_circle: Day 83 (Thursday, 20-07-2023) [Firefighter duty]
Article: "Syslog: The Complete System Administrator Guide"

### :yellow_circle: Day 84 (Friday, 21-07-2023) 
Article: "Monitoring Linux Logs with Kibana and Rsyslog"

### :yellow_circle: Day 85 (Saturday, 22-07-2023) 
I practiced HAProxy with Keeaplived, using nginx as the backend. Everything ran as Docker containers.

### :yellow_circle: Day 86 (Sunday, 23-07-2023) 
Review news about Linux.

### :yellow_circle: Day 87 (Monday, 24-07-2023) 
Testing the MIKR.US VPS.

### :yellow_circle: Day 88 (Thuesday, 25-07-2023) 
Video on YT: "Administracja ElasticSearch dla początkujących"

### :yellow_circle: Day 89 (Wednesday, 26-07-2023) [Firefighter duty] 
Video on YT: "Tworzenie środowiska HA. Narzędzia i przykłady"

### :yellow_circle: Day 90 (Thursday, 27-07-2023) 
**Proxmox Lab**<br/>
Run an NTP server as a Docker container.

### :yellow_circle: Day 91 (Friday, 28-07-2023) 
Configure a Galera Cluster with MariaDB inside Docker containers with Debian.

### :yellow_circle: Day 92 (Saturday, 29-07-2023) [Firefighter duty] 
Video on YT: "Popular Linux interview questions for DevOps interviews"

### :yellow_circle: Day 93 (Sunday, 30-07-2023) 
Review news about Linux.

### :yellow_circle: Day 94 (Monday, 31-07-2023) 
Linux Containers vs Docker - What is the difference?

### :yellow_circle: Day 95 (Thuesday, 01-08-2023) [Firefighter duty] 
Video on YT about "How to run HomeAssistant in Proxmox"

### :yellow_circle: Day 96 (Wednesday, 02-08-2023)
**Proxmox Lab**<br/>
Create an Ansible playbook for configuring hosts as NTP clients.

### :yellow_circle: Day 97 (Thursday, 03-08-2023)
**Proxmox Lab**<br/>
Installation and configuration of the rsyslog server on the 'monitoring' VM.

### :yellow_circle: Day 98 (Friday, 04-08-2023) [Firefighter duty] 
Video on YT: "Proxmox virtual machine automation in Terraform"

### :yellow_circle: Day 99 (Saturday, 05-08-2023)
**Proxmox Lab**<br/>
Configure hosts as rsyslog clients using Ansible playbook.

### :yellow_circle: Day 100 (Sunday, 06-08-2023)
A deeper look into Systemd.

---
**Finished courses during this challenge:**
- "NGINX w godzinę" - Jakub ‘unknow’ Mrugalski
- "Ansible w godzinę" - Jakub ‘unknow’ Mrugalski
- "Administracja Serwerami Linux" - Grupa ADM
- "Akademia Debugowania Linuksa" - Jakub ‘unknow’ Mrugalski

- ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski 

