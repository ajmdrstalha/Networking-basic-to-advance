## 📘 Day 9 – Switching & Routing Basics

### 🔌 1. What is Switching?

**Switching** is the process of **forwarding data within the same network (LAN)** using MAC addresses.

- Works at **Layer 2 (Data Link Layer)**  
- Uses **MAC Address Table (CAM Table)**  
- Connects devices inside a LAN  
- Reduces collision compared to hub  

**Example:**  
PC1 → Switch → PC2 (Same Network)

---

### 🔄 2. How Switching Works

1. Switch receives a frame  
2. Checks **destination MAC address**  
3. Looks into MAC address table  
4. Forwards frame to correct port  

---

### 🧩 3. Types of Switching

| Type | Description |
|------|-------------|
| Store-and-Forward | Checks errors before forwarding |
| Cut-Through | Fast, forwards immediately |
| Fragment-Free | Checks first part before forwarding |

---

### 🔀 4. What is Routing?

**Routing** is the process of **forwarding data packets between different networks** using routers.

- Connects multiple LANs or networks  
- Determines the **best path** for data to reach its destination  
- Works at **Layer 3 (Network Layer)**  

**Example:**  
PC1 (192.168.1.10) → Router → PC2 (192.168.2.10)

---

### 🔢 5. Types of Routing

| Type | Description |
|------|-------------|
| Static Routing | Manually configured routes; fixed paths |
| Dynamic Routing | Routers automatically exchange route information |
| Default Routing | Route used when no specific route exists |

---

### 🔁 6. Routing Table

A **routing table** contains information about paths to reach different networks.

| Destination | Subnet Mask | Gateway | Interface |
|------------|-------------|--------|-----------|
| 192.168.1.0 | 255.255.255.0 | 0.0.0.0 | LAN0 |
| 192.168.2.0 | 255.255.255.0 | 192.168.1.1 | LAN0 |
| 0.0.0.0 | 0.0.0.0 | 192.168.1.254 | WAN0 |

---

### ⚙️ 7. Routing Protocols

| Protocol | Type | Description |
|----------|------|-------------|
| RIP | Distance-vector | Simple, uses hop count |
| OSPF | Link-state | Fast, scalable, uses cost metric |
| EIGRP | Hybrid | Cisco proprietary, efficient |
| BGP | Path-vector | Used on the Internet for inter-domain routing |

---

### 🧪 8. Practical / Lab Practice

- View routing table:

---

### 9. Key Terms

- **Switch:** Connects devices in LAN  
- **Router:** Connects different networks  
- **MAC Address Table:** Stores device MACs  
- **Routing Table:** Stores network paths  
- **Next Hop:** Next router to reach destination  

---

### 📘 Day 9 Summary

✅ Learned switching basics and LAN communication  
✅ Understood routing and inter-network communication  
✅ Explored routing types and protocols  
✅ Practiced routing commands  
