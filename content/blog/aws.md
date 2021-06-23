---
title: "AWS Networking"
author: "Bishwendu Kundu"
date: "2017-01-22T09:00:00"
---

# Regions
AWS provides multiple regions that one can select from, to create their VPC in. Each region has multiple Availability Zones(AZs).

## Virtual Private Cloud
It is an isolated network environment that you have full control over. So as a consumer of AWS you can decide what IP address ranges to choose for your isolated network, how this VPC should divided into smaller subnets and enforce security rules to control how the traffic should inflow/outflow into your subnets. 

### Availability Zones
This is equivalent of say a data center with all the hardware needed to fire up your networks. When you decide to break your VPC into multiple subnets. Each of these subnets can be deployed into any one of AZs within a region. The concept of these zones is to make your application highly available. So this design of separate zones, enables them to fail independently of each other. Now you can deploy your EC2 instance into these subnets.

#### Subnets
A subnet can thought of as a smaller network within the VPC to catering to a very specific type of traffic depending upon your needs.

##### EC2 - Instance
It equivalent of a virtual machine with an OS allowing one to run their applications in. You deploy an EC2 instance into a subnet.