**VanniTech Telecom Enterprise Network Lab**  


<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Focus-CCNA%20Routing%20%26%20Switching-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Tech-Cisco%202911%20%7C%203560--24PS-orange?style=for-the-badge" />
</p>


 **Executive Summary**

This lab is more than a simple Packet Tracer project – it’s a scaled-down enterprise network design meant to reflect **real-world production environments**. It demonstrates mastery of **EIGRP routing, advanced subnetting, routing security, switch configurations, and network scalability planning**.  

VanniTech Telecom’s topology features **departmental segmentation, redundancy-focused design, and pragmatic best practices** – all built with a passion for clean architecture and airtight configs.  

 **My mission with this lab?** To prove that creativity and technical depth can coexist. Networking isn’t just a skillset, it’s a craft.

---

**Network Departments & Roles**

| Department             | Router/Switch | Function                                      |
|-----------------------|-------------|---------------------------------------------|
| Workshop Department    | **R1**      | Edge connectivity and departmental isolation |
| Finance Department     | **R2**      | Core routing and traffic distribution        |
| HR Department          | **R3**      | Branch connectivity and redundancy           |
| Admin Block (HQ)       | **R4 + SW1**| Centralized LAN, gateway, and PC endpoints   |

---

# Topology Highlights  

- **Full-Mesh Interconnectivity:** Every department router communicates seamlessly with low latency.  
- **Hierarchical Subnetting:** `/30` links for WAN efficiency and `/24` for internal LAN scalability.  
- **Routing Security with MD5 Authentication:** Prevents rogue route injections.  
- **Passive Interfaces:** LAN-facing ports silenced to reduce EIGRP chatter.  
- **Loopback Interfaces:** Stability for router IDs, testing, and simulated services.  
- **Switch Optimization:** Port security, VLAN segmentation, and STP optimizations.  

---

## IP Addressing Plan

| Link/Segment            | Subnet         | Devices          |
|------------------------|---------------|-----------------|
| R1 ↔ R2                | `10.0.12.0/30`| Gig0/0 R1 & R2  |
| R1 ↔ R3                | `10.0.13.0/30`| Gig1/0 R1 & R3  |
| R2 ↔ R4                | `10.0.24.0/30`| Gig1/0 R2 & R4  |
| R3 ↔ R4                | `10.0.34.0/30`| Gig0/0 R3 & R4  |
| Admin LAN              | `192.168.4.0/24` | PCs & SW1   |

---

## 🔑 Core Technologies  
| Feature                         | Purpose |
|--------------------------------|---------|
| **EIGRP Routing**               | Dynamic routing, redundancy, scalability |
| **MD5 Key Authentication**      | Secure routing exchanges |
| **VLAN Segmentation**           | Department-based access control |
| **Access Port Hardening**       | STP PortFast, Port Security |
| **Subnetting Strategy**         | Efficient address planning |
| **Router/Switch Banners**       | Security compliance messaging |
| **Login Security**              | VTY password protection & key chains |

---

##  Skills Demonstrated

- Cisco IOS CLI mastery across Routers & L3 Switches  
- End-to-end network design (logical + physical)  
- Subnetting / IP hierarchy expertise  
- Routing protocol optimization and security  
- Device hardening & baseline security practices  
- GitHub documentation for technical projects  

---

##  Future Enhancements

📌 Because true network engineers never stop improving:  

- IPv6 Dual-Stack Deployment  
- Implementation of ACLs & Firewalls  
- QoS Policies for Voice & Video  
- Redundant Gateway Failover (HSRP/VRRP)  
- SNMP Monitoring & Centralized Syslog  

---

## 🧑‍💻 About the Author

Hi, I’m **Bradley Giovanni** – a networking enthusiast on a mission to turn theory into practical, production-grade solutions. Currently pursuing **CCNA certification**, I thrive in designing and documenting clean, scalable networks while staying obsessed with every CLI detail.  

> “Networking isn’t just a career path – it’s an artform. This lab reflects my hunger for mastery.”  

EMAIL: giovanniibradley@gmail.com

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/bradley-giovanniii293)
---
