# Overview

# Setup
### What I used: 
- Raspberry Pi Zero 2 W
- Pi-hole
- Micro SD (for operating system)
- Micro SD reader (for writing operating system to micro SD)
- Micro USB (for powering the Pi)
- Computer (to write operating system to micro SD)

### Steps:
- 
# How it works
### Pi-hole
Pi-hole is a DNS sinkhole that protects your devices from unwanted content. A DNS sinkhole acts as a DNS server that checks each requested domain against blocklists (and optionally allowlists). If the domain is allowed, Pi-hole forwards the query to an upstream DNS server and returns the real IP address. If the domain is blocked, Pi-hole instead returns a non-routable address (like `0.0.0.0`), effectively preventing the connection.
