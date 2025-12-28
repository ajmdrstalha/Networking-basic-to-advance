## 📘 Day 9 – Routing Basics

### 🧩 1. What is Routing?

**Routing** is the process of **forwarding data packets between different networks** using routers.

- Connects multiple LANs or networks  
- Determines the **best path** for data to reach its destination  
- Works at **Layer 3 (Network Layer)**  

Example:
PC1 (192.168.1.10) → Router → PC2 (192.168.2.10)

yaml
Copy code

---

### 🔢 2. Types of Routing

| Type | Description |
|------|-------------|
| Static Routing | Manually configured routes; fixed paths |
| Dynamic Routing | Routers automatically exchange route information |
| Default Routing | Route used when no specific route exists |

---

### 🔁 3. Routing Table

A **routing table** contains information about paths to reach different networks.

Example (simplified):

| Destination | Subnet Mask | Gateway | Interface |
|------------|-------------|--------|-----------|
| 192.168.1.0 | 255.255.255.0 | 0.0.0.0 | LAN0 |
| 192.168.2.0 | 255.255.255.0 | 192.168.1.1 | LAN0 |
| 0.0.0.0 | 0.0.0.0 | 192.168.1.254 | WAN0 |

---

### ⚙️ 4. Routing Protocols

| Protocol | Type | Description |
|----------|------|-------------|
| RIP | Distance-vector | Simple, uses hop count |
| OSPF | Link-state | Fast, scalable, uses cost metric |
| EIGRP | Hybrid | Cisco proprietary, efficient |
| BGP | Path-vector | Used on the Internet for inter-domain routing |

---

### 🗂️ 5. Practical / Lab Practice

- View routing table on devices:

**Windows:**
route print

makefile
Copy code

**Linux:**
ip route show

markdown
Copy code

- Add static route:

**Windows:**
route add 192.168.2.0 mask 255.255.255.0 192.168.1.1

yaml
Copy code

- Test connectivity with `ping` and `tracert/traceroute`

---

### 🧠 6. Key Terms

- **Router:** Device that forwards packets between networks  
- **Routing Table:** Stores network paths  
- **Static Route:** Manually configured path  
- **Dynamic Route:** Learned automatically via protocol  
- **Next Hop:** Next router to reach destination network  

---

### 📘 Day 9 Summary

✅ Learned what routing is and its importance  
✅ Explored types of routing  
✅ Understood routing tables and protocols  
✅ Practiced viewing and configuring routes  
