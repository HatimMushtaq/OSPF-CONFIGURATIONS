# OSPF Network Simulation – Cisco Packet Tracer

## 📘 Project Overview
This project demonstrates the configuration and operation of **Open Shortest Path First (OSPF)** routing in a simulated network environment using **Cisco Packet Tracer**.  
The main purpose of this project is to **recall and strengthen OSPF configuration and troubleshooting skills**.

## 🧠 Objective
The objective of this project is to:
- Design a multi-area OSPF network.
- Establish inter-router communication.
- Optimize routing using hierarchical OSPF areas.
- Verify connectivity and route propagation between all routers and end devices.

## 🏗️ Network Topology
- **Routers:** 4  
- **Switches:** (optional depending on host connection)  
- **End Devices (PCs):** Multiple (to test connectivity)  
- **Routing Protocol:** OSPF (Multi-Area Configuration)  

### Example Areas
- **Area 0:** Backbone area  
- **Area 1, Area 2:** Connected sub-areas for branch networks

## ⚙️ Tools Used
- **Cisco Packet Tracer** (Version 8.x or later)  
- **Operating System:** Windows/Linux/MacOS  
- **Routing Protocol:** OSPF (Open Shortest Path First)

## 🧩 Configuration Summary
Each router is configured with:
- OSPF process ID  
- Router IDs  
- Network statements defining participating interfaces  
- Area assignments for hierarchical routing  
- (Optional) Passive interfaces and OSPF authentication  

Example CLI snippet:
```bash
Router(config)# router ospf 1
Router(config-router)# router-id 1.1.1.1
Router(config-router)# network 192.168.1.0 0.0.0.255 area 0
Router(config-router)# network 10.0.0.0 0.0.0.255 area 1
