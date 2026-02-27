# ENCS304 - Computer Networks  
## Lab Assignment 1  
### Basic Network Topologies Using Switches and Hubs  

---

## 📌 Student Details
- **Name:** Nitesh Sharma  
- **Roll No:** 2301010151  
- **Program:** B.Tech CSE  
- **Section:** C  
- **Faculty:** Mr. Mohammad Aijaz  

---

## 🎯 Objectives

The objective of this lab is to design, configure, and analyse three fundamental LAN topologies using Cisco Packet Tracer:

- Star Topology using a Switch  
- Bus-like Topology using a Hub  
- Ring-like Topology using 3 Switches  
- Link Failure Test with STP reconvergence  

The experiment evaluates:
- Connectivity using ICMP ping  
- Collision behaviour  
- Traffic handling  
- Fault tolerance  

---

## 🛠 Tools & Technologies Used

- Cisco Packet Tracer  
- 2960-24TT Switch  
- Hub-PT  
- IPv4 Addressing (192.168.10.0/24)  
- ICMP Ping Testing  
- Spanning Tree Protocol (STP)  

---

## 🌐 Network Configurations

All devices were configured in the same subnet:

| Device Range | Subnet |
|-------------|--------|
| 192.168.10.1 – 192.168.10.5 | 255.255.255.0 |

---

## 🔷 Task 1: Star Topology (Switch)

- 4 PCs connected to a 2960 switch  
- Unicast forwarding  
- No collisions  
- 0% packet loss  
- <1ms latency  

✅ Best general-purpose performance  

---

## 🔷 Task 2: Bus-like Topology (Hub)

- 4 PCs connected to Hub  
- Single shared collision domain  
- Broadcast behaviour observed  
- 0% packet loss (under sequential testing)  

⚠ Not suitable for high traffic environments  

---

## 🔷 Task 3: Ring-like Topology (3 Switches)

- 3 switches connected in triangular loop  
- STP blocks one port (prevents broadcast storm)  
- Full cross-switch connectivity  
- 0% packet loss  

✅ Redundant path available  

---

## 🔥 Task 4: Link Failure Test

- Cable between SwitchA and SwitchB removed  
- STP reconverged automatically  
- Alternate path activated instantly  
- 0% packet loss after failover  

✅ Demonstrates fault tolerance  

---

## 📊 Comparative Analysis

| Aspect | Star | Hub | Ring |
|--------|------|------|------|
| Collision Domain | Isolated | Shared | Isolated |
| Traffic Type | Unicast | Broadcast | Unicast |
| Fault Tolerance | No | No | Yes |
| Real-world Usage | Office LAN | Legacy | Data Centers |

---

## 🧠 Conclusion

- Star topology is ideal for standard office LANs.  
- Hub-based topology is obsolete due to shared collision domain.  
- Ring topology with STP provides redundancy and high availability.  

Switch-based networks are recommended for modern infrastructure due to efficiency and scalability.

---

## 📂 Repository Contents

- Lab Report (PDF)  
- Cisco Packet Tracer (.pkt) file  
- README Documentation  

---
