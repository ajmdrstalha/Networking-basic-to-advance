## 📘 Day 7 – Ports & Protocols

### 🧩 1. What are Ports?

A **port** is a logical endpoint in a network used to identify a specific process or service on a device.

- Works at **Transport Layer (TCP/UDP)**  
- Helps multiple services run on the same IP  
- Each port has a **number** from 0–65535  

Types of Ports:

| Type | Range | Usage |
|------|-------|-------|
| Well-known | 0–1023 | Standard services like HTTP, FTP, SMTP |
| Registered | 1024–49151 | Vendor-specific applications |
| Dynamic/Private | 49152–65535 | Temporary or client-assigned ports |

---

### 🔢 2. Common TCP/UDP Ports

| Port | Protocol | Service |
|------|----------|--------|
| 20/21 | TCP | FTP (File Transfer) |
| 22 | TCP | SSH (Secure Shell) |
| 23 | TCP | Telnet |
| 25 | TCP | SMTP (Mail) |
| 53 | UDP/TCP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 443 | TCP | HTTPS |

---

### 🔁 3. TCP vs UDP

| Feature | TCP | UDP |
|---------|-----|-----|
| Connection | Connection-oriented | Connectionless |
| Reliability | Guaranteed delivery | No guarantee |
| Error Checking | Yes | Minimal |
| Use Cases | Web, email, file transfer | Streaming, gaming, DNS queries |

---

### ⚙️ 4. How Ports Work

1. Application binds to a port on a host  
2. Client sends a request to server’s IP and port  
3. Server listens on the port and responds  
4. Multiple services can run on same IP using different ports  

---

### 🗂️ 5. Practical / Lab Practice

- Use `netstat -an` to view open ports and active connections  
- Use `telnet IP PORT` to test connectivity to a service  
- Identify which services are running using port numbers  

---

### 🧠 6. Key Terms

- **Port Number:** Identifies a process or service  
- **Socket:** Combination of IP + Port  
- **Well-known Ports:** Standard service ports  
- **Dynamic Ports:** Temporary client ports  

---

### 📘 Day 7 Summary

✅ Learned what ports are and their types  
✅ Explored common TCP/UDP ports  
✅ Understood TCP vs UDP differences  
✅ Practiced checking and testing ports 
