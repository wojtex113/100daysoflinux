Hi all,

My name's Wojtek and I own business called 'WOJST Usługi Informatyczne Wojciech Stańczyk' with a website https://wojst.pl<br/>
I write my thoughts, tips and another IT notes on the blog, which can be found at https://wojst.pl/blog

Today (29-04-2023) I've started the #100DaysOfLinux challenge. My goal is to finish all courses I have purchased but haven't yet completed and complete many labs during this time.

I aspire to be a Linux Administrator, which is my main goal, and I'm also considering the possibility of working in Dev/Ops.

Additionaly, I'm a firefighter in Państwowa Straż Pożarna, where we work 24-hour shifts every three days. During my shifts I will try found a few minutes to read or watch something related to this challenge.

So, let's get started :)

--<br/>
var ASL = course 'Administracja Serwerami Linux' by Grupa ADM<br/>

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

### :yellow_circle: Day 12 (Wendesday, 10-05-2023)
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

### :yellow_circle: Day 19 (Wendesday, 17-05-2023)
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

---
**Finished courses:**
- "NGINX w godzinę" - Jakub ‘unknow’ Mrugalski
- "Ansible w godzinę" - Jakub ‘unknow’ Mrugalski

- ebook '77 zadań dla adminów' by Jakub ‘unknow’ Mrugalski 

