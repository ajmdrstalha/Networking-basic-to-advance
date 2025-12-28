## 📘 Day 18 – Router Configuration Basics

### 🧩 1. What is a Router?

A **router** is a network device that **connects multiple networks** and forwards data packets based on **IP addresses**.

- Operates at **Layer 3 (Network Layer)**  
- Determines the best path for data using routing tables  
- Connects LANs to WANs or the Internet  

Example:
- Connecting an office LAN to the Internet  
- Connecting multiple branch networks  

---

### 🔢 2. Types of Routers

| Type | Description |
|------|-------------|
| Home Router | Simple router for home networks, usually with NAT and Wi-Fi |
| Enterprise Router | Advanced features for businesses, supports multiple interfaces and routing protocols |
| Core Router | High-capacity router used in the backbone of large networks |
| Edge Router | Connects internal network to external networks/Internet |

---

### 🔁 3. Basic Router Operations

- Forwarding packets between networks  
- Maintaining routing tables  
- Performing NAT and PAT for private networks  
- Supporting security features (firewall, ACLs)  

---

### ⚙️ 4. Router CLI Commands (Cisco Example)

- Access router CLI via console or SSH  
- Common commands:

enable # Enter privileged mode
configure terminal # Enter global config mode
hostname Router1 # Set router name
interface gig0/0
ip address 192.168.1.1 255.255.255.0
no shutdown # Enable interface
show running-config # View current configuration
show ip route # View routing table
ping 192.168.1.2 # Test connectivity

yaml
Copy code

---

### 🗂️ 5. Practical / Lab Practice

- Assign IP addresses to router interfaces  
- Connect LAN devices to the router and test connectivity  
- Configure static routes between networks  
- Test routing using `ping` and `traceroute`  
- Observe routing table and interface status  

---

### 🧠 6. Key Terms

- **Interface:** Network port on the router  
- **Routing Table:** Stores paths to networks  
- **Static Route:** Manually configured route  
- **Dynamic Route:** Learned automatically via routing protocol  
- **NAT/PAT:** Translate private IPs to public IPs  

---

### 📘 Day 18 Summary

✅ Learned what a router is and its purpose  
✅ Explored types of routers  
✅ Practiced basic router configuration  
✅ Verified routing and connectivity in the network  
