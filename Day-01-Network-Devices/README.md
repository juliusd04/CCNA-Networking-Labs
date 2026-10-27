# Day 1 - Network Devices

## Objective
The objective of this lab was to understand the
functions of different networking devices and
how they connect clients and servers across
different locations.

## Tools Used
- Cisco Packet Tracer

## Network Scenario
This lab involved two separate locations:

- New York Branch: Contained client devices.
- Tokyo Branch: Contained servers.

The goal was to identify and place the
appropriate networking devices to connect
the New York branch to the Tokyo branch.

## Lab Activities
- Examined the existing network topology.
- Identified the client devices and servers.
- Determined which networking devices were
  needed to connect the two locations.
- Added the appropriate networking devices
  to the topology.

## Concepts Practiced
- Network devices and their functions
- Client-server networks
- Local Area Networks (LANs)
- Wide Area Networks (WANs)
- Basic network topology design

## What I Learned
This lab helped me understand how different
networking devices work together to connect
computers and servers across multiple locations.

I also gained experience identifying the
networking equipment needed to establish
connections between different networks.

## Network Topology

The screenshot below shows my completed Day 1
network topology in Cisco Packet Tracer.

The topology includes client devices at the
New York branch and servers at the Tokyo branch.

![Day 1 Network Topology](Screenshot%202026-10-27%20153839.png)

## Network Devices and Their Functions

### End Devices
- **PCs:** Represent client devices at the New York branch.
- **Servers:** Represent network resources located at the Tokyo branch.
- **Laptop:** Represents a potential external attacker connected to the simulated Internet.

### Switches
- Cisco 2960 switches connect devices within each branch's local network.
- Switches forward Ethernet frames using MAC addresses.

### Routers
- Cisco 2911 routers connect different networks.
- Routers forward IP packets between networks using routing information.
- The central router represents the Internet in this simplified topology.

### Firewalls
- Cisco ASA 5505 firewalls are included at both branches.
- Firewalls can control network traffic according to configured security policies.
- They help protect internal networks from unauthorized access.

## Network Design

The topology demonstrates how client devices in
New York could communicate with servers in Tokyo
through interconnected networking devices.

The lab focused on identifying and placing the
appropriate devices rather than configuring
routing protocols or firewall security policies.

## Key Takeaways

- Switches connect devices within local networks.
- Routers provide connectivity between different networks.
- Firewalls can filter traffic between network segments.
- Servers provide resources and services to clients.
- Network topology diagrams help visualize how devices
  are interconnected.
