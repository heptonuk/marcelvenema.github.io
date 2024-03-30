---
title: "Homelab upgrade!"
date: 2022-09-24T09:00:00+01:00
draft: true
tags: ["devops"]
author: "marcelvenema"
---

Last week I upgraded my home lab with a real physical server :-) Thanks to the fine folks at [CreoServer.com](http://creoserver.com/), I purchased a refurbished 14th-generation Dell PowerEdge R640LFF rack server.

When you are wondering, why purchase a physical server when you can create a virtual server with one or two clicks in the cloud: 

Some of my software projects are about installing hypervisors on physical hardware. A real physical development server helps.

Some of my customers are on-premises only.

It looks cool in your home lab.

Because I can.


My first project is installing Nutanix on the physical server. It will be a single-node cluster as purchasing the normal cluster size, three physical servers, definitely will break the bank and cause a divorce.  The Nutanix [hardware compatibility list](https://portal.nutanix.com/page/documents/details?targetId=Dell-Hardware-Firmware-Compatibility:Dell-Hardware-Firmware-Compatibility) is very strict, especially on HPE and Dell. The budget is limited and I ended up with a Dell R640 LFF PowerEdge server with a dual Intel Xeon 4116 Silver CPU @2.10Ghz, 192GB RAM memory, an Intel 10G X710/i350 4 port NIC and hybrid storage of two 980GB SATA SSD drives and two 4TB SATA HDD drives.  

It was very kind of [CreoServer.com](http://creoserver.com/) that it was possible to do some initial testing of the server in their showroom. One of the first findings was the requirement of the iDRAC9 Enterprise license. It is mentioned in the HCL but the server came with an iDRAC9 Basic license. I ordered an iDRAC9 Enterprise license and in the meanwhile used a free 30days trial license to proceed testing. I also forgot to order two 2.5" SFF to 3.5" LFF conversion adapters for the SSD disks.  


In another blog post I will write about the installation of Nutanix with the help of Nutanix Portable Foundation app. 



Disclaimer: This blog post and mentioned hardware are NOT sponsored. Paid with my own money.

 
