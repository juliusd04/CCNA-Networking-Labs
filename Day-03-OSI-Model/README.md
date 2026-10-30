# Day 3 - TCP/IP and OSI Models

## Overview

In this lab, I used Cisco Packet Tracer to explore how network protocols operate across different layers of the OSI and TCP/IP models. Using Simulation Mode, I observed how devices communicate and how protocols such as ARP and ICMP are used during network communication.

I also performed additional networking experiments using Windows Command Prompt to better understand how these concepts apply to real-world networks.

## Tools Used

- Cisco Packet Tracer
- Windows Command Prompt
- Jeremy's IT Lab CCNA Course

---

## Part 1 - Packet Tracer Lab

### Objective

Understand how network communication occurs across different layers of the OSI model by observing protocols and packet exchanges in Cisco Packet Tracer.

### Lab Activities

1. Opened the provided network topology in Cisco Packet Tracer.
2. Used PC1's Command Prompt to ping the server at `192.168.1.100`.
3. Enabled Simulation Mode to observe network communication.
4. Examined ARP and ICMP events as packets traveled through the network.
5. Observed how different protocols operate at different layers of the OSI model.

### Protocols Observed

**ARP (Address Resolution Protocol)**

ARP is used to resolve IPv4 addresses to MAC addresses on a local network. Before sending an Ethernet frame, a device may need to discover the MAC address associated with the destination IP address or its default gateway.

**ICMP (Internet Control Message Protocol)**

ICMP is used for network diagnostics and error reporting. The `ping` command uses ICMP Echo Requests and Echo Replies to test network connectivity.

**STP (Spanning Tree Protocol)**

STP is a Layer 2 protocol that helps prevent switching loops in networks with redundant connections. STP events were also visible in the Packet Tracer simulation.

### Key Takeaways

- Network communication involves multiple protocols working together.
- ARP helps devices determine the appropriate destination MAC address.
- ICMP allows devices to test network connectivity.
- Switches forward Ethernet frames using MAC addresses.
- Packet Tracer's Simulation Mode helps visualize how network protocols operate.

---

## Part 2 - Independent Networking Experiments

After completing the TCP/IP and OSI model lessons, I experimented with networking commands on my personal computer to better understand how devices communicate across the Internet.

### Experiment 1 - Tracing Network Routes

**Commands Used:**

```cmd
tracert nike.com
tracert -d nike.com
```

I used `tracert` to examine the route between my computer and Nike's website.

The results showed multiple intermediate routers, including routers associated with my Internet service provider, Comcast.

I learned that:

- Packets can travel through multiple routers before reaching their destination.
- Each router represents a Layer 3 hop along the network path.
- The `-d` option displays IP addresses without performing reverse DNS lookups.
- Some routers may not respond to traceroute probes, resulting in timeouts.
- Traceroute uses increasing TTL values to identify intermediate routers.

### Experiment 2 - Comparing IPv4 and IPv6

**Commands Used:**

```cmd
tracert -4 resurgens.com
tracert -6 resurgens.com
```

I compared IPv4 and IPv6 traceroutes to the same website.

The results showed that the network paths and addressing formats could differ depending on which Internet Protocol version was used.

I also learned how to distinguish IPv6 addresses from MAC addresses, since both use hexadecimal notation.

### Experiment 3 - DNS Resolution

**Command Used:**

```cmd
nslookup resurgens.com
```

I used `nslookup` to identify the IP addresses associated with the website.

The results showed that my computer was using a Comcast DNS resolver.

I learned that:

- DNS translates domain names into IP addresses.
- DNS A records contain IPv4 addresses.
- DNS AAAA records contain IPv6 addresses.
- A DNS resolver is different from the web server hosting a website.
- A domain can resolve to multiple IPv4 and IPv6 addresses.

The lookup also showed that the website uses Cloudflare infrastructure.

### Experiment 4 - Testing Network Connectivity

**Command Used:**

```cmd
ping cdns01.comcast.net
```

I used `ping` to test connectivity to Comcast's DNS server.

The server responded using IPv6, allowing me to observe round-trip times and confirm that ICMP Echo Requests and Echo Replies were being exchanged.

I learned that ping can test IPv4 and IPv6 connectivity, but a failed ping does not necessarily mean a device is offline because firewalls and network policies may block ICMP traffic.

---

## Connecting the Concepts

These experiments helped me understand how the OSI and TCP/IP models apply to actual network communication.

For example, when accessing a website:

1. DNS can resolve the domain name into an IP address.
2. The computer determines whether the destination is on the local network or requires a default gateway.
3. ARP may be used to discover the MAC address of the next-hop device when communicating over IPv4 Ethernet.
4. Routers forward IP packets toward the destination.
5. ICMP can be used to test connectivity and identify routers along a network path.

The Packet Tracer simulation helped me visualize these processes, while the Command Prompt experiments allowed me to observe them on my actual network.

## Conclusion

This lab strengthened my understanding of the TCP/IP and OSI models, network
