## 📘 Day 11 – Firewall Basics

### 🧩 1. What is a Firewall?

A **firewall** is a network security device or software that **monitors and controls incoming and outgoing network traffic** based on predefined rules.

- Protects networks from unauthorized access  
- Can be hardware, software, or cloud-based  
- Works at **Layer 3 (Network) and Layer 4 (Transport)**  

Example:
- Allow HTTP/HTTPS traffic  
- Block suspicious IP addresses  

---

### 🔢 2. Types of Firewalls

| Type | Description |
|------|-------------|
| Packet Filtering | Filters traffic based on IP, protocol, or port |
| Stateful Inspection | Monitors active connections and packet states |
| Proxy Firewall | Acts as an intermediary for requests |
| Next-Generation Firewall (NGFW) | Includes advanced features like IPS, application control |

---

### 🔁 3. Firewall Rules

- Rules define **what traffic is allowed or blocked**  
- Usually follow **allow/deny order**  
- Common elements:
  - Source IP / Destination IP  
  - Source Port / Destination Port  
  - Protocol (TCP/UDP/ICMP)  
  - Action (Allow / Deny / Drop)  

---

### ⚙️ 4. How Firewalls Work

1. Packet enters the network  
2. Firewall examines packet headers and content  
3. Checks against rule set  
4. Allows or blocks traffic based on rules  

---

### 🗂️ 5. Practical / Lab Practice

- Check firewall status:

**Windows:**
netsh advfirewall show allprofiles

markdown
Copy code

**Linux (iptables):**
sudo iptables -L -v -n

yaml
Copy code

- Test blocking/allowing a port using firewall rules  
- Observe allowed and blocked traffic  

---

### 🧠 6. Key Terms

- **Packet Filtering:** Basic firewall functionality  
- **Stateful Inspection:** Tracks connection states  
- **Proxy Firewall:** Acts as intermediary  
- **NGFW:** Advanced firewall with multiple features  
- **Rule Set:** Defines allowed or blocked traffic  

---

### 📘 Day 11 Summary

✅ Learned what a firewall is and its importance  
✅ Explored types of firewalls  
✅ Understood firewall rules and how they work  
✅ Practiced checking and configuring firewall rules  
