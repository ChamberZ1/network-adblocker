# Overview

In the digital age, data gathering, tracking, and ads are massive revenue streams for corporate giants. Roughly ~75% of Google’s revenue and ~98% of Meta’s revenue come from advertising, so it’s no surprise that the modern web is packed with trackers and junk we never asked for.

For people who value privacy and cleaner pages, tools like Pi-hole (and the uBlock Origin browser extension, though that’s outside the scope of this project) can make a huge difference. Pi-hole is a DNS-based filtering tool, designed for Linux systems, that’s primarily used as a network-wide ad and tracker blocker.

In this repo, I document my process of:

- Setting up a Raspberry Pi Zero 2 W  
- Installing and configuring the OS  
- Installing Pi-hole  
- Wiring it into my home network so all local DNS traffic runs through it

The goal is to end up with a low-power Raspberry Pi acting as a dedicated DNS sinkhole for my home network, giving me network-wide ad blocking while I learn more about DNS, Linux, and basic homelab/network setup.

# How it works
### Pi-hole
Pi-hole is a DNS sinkhole that protects your devices from unwanted content. A DNS sinkhole acts as a DNS server that checks each requested domain against blocklists (and optionally allowlists). If the domain is allowed, Pi-hole forwards the query to an upstream DNS server and returns the real IP address. If the domain is blocked, Pi-hole instead returns a non-routable address (like `0.0.0.0`), effectively preventing the connection.

### Diagram
![Diagram of home network with Pi-hole](Pi-hole diagram.png)

# Setup
### What I used: 
- Raspberry Pi Zero 2 W
- Pi-hole
- Micro SD (for operating system)
- Micro SD reader (for writing operating system to micro SD)
- Micro USB (for powering the Pi)
- Computer (to write operating system to micro SD)

### Steps:
1) 

2) 

# Acknowledgements
- [WesOps](https://www.youtube.com/watch?v=d_3h5n9mPdI) on YouTube. His video was what introduced me to Pi-hole and inspired me to give this a try.
- [Pi-hole](https://pi-hole.net/)
