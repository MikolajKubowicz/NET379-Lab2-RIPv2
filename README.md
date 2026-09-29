# Cisco Routing Lab – RIPv2 Dynamic Routing

This project demonstrates the configuration and troubleshooting of a multi-router network using Cisco Modeling Labs (CML).

I built a four-router topology, assigned IPv4 addressing across multiple subnets and loopback interfaces, and configured RIP version 2 as the dynamic routing protocol. I then tested connectivity before and after routing was enabled to observe how routers learn remote networks and update their routing tables.

## What I Implemented

- Configured IPv4 addressing on Cisco router interfaces
- Created and configured loopback interfaces
- Configured RIP version 2 across four routers
- Verified connectivity using `ping`
- Analyzed routing tables using `show ip route`
- Compared routing behavior with automatic summarization enabled and disabled
- Identified equal-cost routes with multiple next hops
- Tested the effect of interface bandwidth changes on RIP route selection
- Exported and preserved the completed topology using Cisco Modeling Labs YAML

## Key Networking Concepts

This project reinforced several important networking concepts:

- Dynamic routing
- Routing tables
- Directly connected vs. learned routes
- RIP hop-count metrics
- Route summarization
- Equal-Cost Multi-Path routing
- IPv4 subnetting
- Network troubleshooting

## Technical Environment

- Cisco Modeling Labs (CML)
- Cisco IOS
- RIP version 2
- IPv4
- Command-line interface configuration

## Example Commands

```bash
show ip interface brief
show ip route
ping <destination-ip>

router rip
version 2
network 10.0.0.0
no auto-summary
