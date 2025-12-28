## 📘 Day 29 – Introduction to Firewalls & ACLs

### 🧩 1. What is a Firewall?

A **firewall** is a network security device or software that **monitors and controls incoming and outgoing traffic** based on security rules.

- Protects networks from unauthorized access and attacks  
- Can be hardware-based, software-based, or cloud-based  
- Operates at different layers (Packet Filtering, Stateful, Application)  

Example:
- Blocking specific IP addresses or ports  
- Allowing only certain applications to access the Internet  

---

### 🔢 2. Types of Firewalls

| Type | Description |
|------|-------------|
| Packet Filtering | Examines packets and allows/blocks based on IP, port, protocol |
| Stateful Inspection | Tracks the state of active connections for better security |
| Proxy Firewall | Intermediary between users and external network, inspects traffic |
| Next-Generation Firewall (NGFW) | Adds application awareness, intrusion prevention, and threat intelligence |

---

### 🔁 3. What is an ACL?

**ACL (Access Control List)** is a set of **rules applied on routers or firewalls** to permit or deny traffic.

- Can filter based on IP, protocol, port, or interface  
- Supports inbound and outbound filtering  
- Enhances security and traffic control  

Example:
- Deny all traffic from a specific IP  
- Allow only HTTP/HTTPS traffic to a web server  

---

### ⚙️ 4. Basic ACL Commands (Cisco Example)

- Configure standard ACL:
access-list 10 permit 192.168.1.0 0.0.0.255
interface gig0/0
ip access-group 10 in

diff
Copy code

- Configure extended ACL:
access-list 100 permit tcp any host 192.168.1.10 eq 80
interface gig0/0
ip access-group 100 in

diff
Copy code

- Verify ACLs:
show access-lists
show ip interface

yaml
Copy code

---

### 🗂️ 5. Practical / Lab Practice

- Apply standard and extended ACLs on a router  
- Test traffic filtering using `ping` and `telnet`  
- Configure a firewall to allow only specific services  
- Monitor allowed and denied traffic  
- Document ACL rules and verify functionality  

---

### 🧠 6. Key Terms

- **Firewall:** Security device controlling network traffic  
- **ACL:** List of rules permitting or denying traffic  
- **Inbound/Outbound:** Direction of traffic relative to the device  
- **Packet Filtering:** Basic firewall method checking headers  
- **NGFW:** Advanced firewall with application awareness  

---

### 📘 Day 29 Summary

✅ Learned firewall fundamentals and types  
✅ Explored ACL concepts and configurations  
✅ Practiced applying ACLs and firewall rules  
✅ Understood traffic control and network security enforcement 
