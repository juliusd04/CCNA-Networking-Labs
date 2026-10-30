# Day 2 - Connecting Network Devices

## Overview
In this lab, I used Cisco Packet Tracer to practice connecting different network devices using the appropriate Ethernet and fiber optic cables. The objective was to understand how different devices are physically connected and how cable selection depends on device types and transmission distances.

## Lab Objectives
- Identify the appropriate cables for connecting network devices.
- Understand the differences between straight-through and crossover Ethernet cables.
- Learn when to use single-mode and multimode fiber optic cables.
- Connect routers, switches, PCs, and servers in a network topology.

## Tools Used
- Cisco Packet Tracer
- Jeremy's IT Lab CCNA Course

## Lab Activities

### 1. Connecting End Devices
I connected PCs and servers to switches using copper straight-through cables. These cables are commonly used when connecting different types of Ethernet devices.

### 2. Connecting Switches
I used copper crossover cables to connect switches to other switches. The lab assumed Auto MDI-X was disabled, meaning the appropriate cable type needed to be selected manually.

### 3. Connecting Routers
I connected routers and switches using the appropriate Ethernet cables. I also practiced selecting fiber optic cables for connections between routers at different distances.

The lab included the following router connections:

- R1 to R2: 50 meters
- R1 to R3: 3 kilometers
- R3 to R4: 250 meters

### 4. Understanding Fiber Optic Connections
I learned that single-mode fiber is generally more suitable for long-distance connections, while multimode fiber is commonly used for shorter distances.

For the 3-kilometer connection between R1 and R3, single-mode fiber would generally be the appropriate real-world choice. However, Packet Tracer did not allow me to connect single-mode fiber to the selected GigabitEthernet interface, so I used multimode fiber to complete the simulated connection.

For the 250-meter connection between R3 and R4, I used multimode fiber.

## Key Takeaways
- Straight-through cables are commonly used between different types of Ethernet devices.
- Crossover cables are used between similar Ethernet devices when Auto MDI-X is unavailable.
- Fiber optic cable selection depends on distance and hardware compatibility.
- Single-mode fiber is generally better suited for longer distances.
- Packet Tracer has limitations that may differ from real-world networking equipment.

## Conclusion
This lab helped me better understand physical network connections and the importance of selecting appropriate cables. It also introduced me to hardware compatibility considerations when working with fiber optic connections.
