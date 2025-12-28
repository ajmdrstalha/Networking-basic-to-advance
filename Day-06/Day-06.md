## 📘 Day 6 – OSI & TCP/IP Models

### 🧩 1. What is OSI Model?

The **OSI (Open Systems Interconnection) model** is a conceptual framework to understand **how data travels across networks**.

- Divides network communication into **7 layers**  
- Helps in troubleshooting and designing networks  
- Each layer has a specific function  

Layers of OSI (from top to bottom):

| Layer | Function |
|-------|---------|
| Application | Provides network services to applications |
| Presentation | Data translation, encryption, compression |
| Session | Manages sessions and connections |
| Transport | Ensures reliable data transfer (TCP/UDP) |
| Network | Routing and addressing (IP) |
| Data Link | MAC addressing, error detection |
| Physical | Physical transmission of data (cables, signals) |

---

### 🔢 2. OSI Layer Details

1. **Physical Layer** – Cables, switches, bits transmission  
2. **Data Link Layer** – MAC addresses, frames, error detection  
3. **Network Layer** – IP addressing, routing  
4. **Transport Layer** – TCP/UDP, ensures complete data delivery  
5. **Session Layer** – Session management between devices  
6. **Presentation Layer** – Data formatting, encryption  
7. **Application Layer** – Interfaces for applications like HTTP, FTP, DNS  

---

### 🔁 3. TCP/IP Model

The **TCP/IP model** is a simpler, practical model used on the Internet.

| Layer | OSI Equivalent | Function |
|-------|----------------|---------|
| Application | Application, Presentation, Session | Network services for apps |
| Transport | Transport | TCP/UDP, reliable or connectionless communication |
| Internet | Network | IP addressing, routing |
| Network Access / Link | Data Link + Physical | Hardware addressing, physical transmission |

---

### ⚙️ 4. OSI vs TCP/IP

| Feature | OSI | TCP/IP |
|---------|-----|--------|
| Layers | 7 | 4 |
| Usage | Conceptual, teaching | Practical, Internet |
| Protocols | Layer-specific | Integrated into layers |
| Flexibility | High | Medium |

---

### 🗂️ 5. Practical / Lab Practice

- Identify which OSI layer a protocol belongs to (HTTP → Application, TCP → Transport)  
- Use `ping` to test Network layer connectivity  
- Use `traceroute/tracert` to observe routing at the Network layer  

---

### 🧠 6. Key Terms

- **Frame:** Data unit at Data Link layer  
- **Packet:** Data unit at Network layer  
- **Segment:** Data unit at Transport layer  
- **Protocol:** Rules for communication  
- **Encapsulation:** Wrapping data with headers at each layer  

---

### 📘 Day 6 Summary

✅ Learned OSI 7 layers and functions  
✅ Understood TCP/IP 4 layers and mapping to OSI  
✅ Compared OSI vs TCP/IP models  
✅ Practiced identifying protocols and data units  
