## 📘 Day 14 – Network Troubleshooting Basics

### 🧩 1. What is Network Troubleshooting?

**Network Troubleshooting** is the process of **identifying, diagnosing, and resolving network issues**.

- Ensures connectivity and performance  
- Helps prevent downtime and errors  
- Uses tools, commands, and systematic steps  

Example:
- Unable to access the Internet  
- Slow network speed  
- IP conflicts  

---

### 🔢 2. Common Network Issues

| Issue | Possible Cause |
|-------|----------------|
| No connectivity | Wrong IP, disconnected cable, AP down |
| Slow network | Bandwidth congestion, interference, overloaded devices |
| IP conflicts | Duplicate IP addresses on the network |
| DNS failure | Incorrect DNS settings, server issues |
| Firewall blocks | Port blocked or rules misconfigured |

---

### 🔁 3. Troubleshooting Steps

1. Identify the problem  
2. Gather information (IP config, ping, traceroute)  
3. Isolate the issue (device, cable, switch, router)  
4. Test solutions and verify connectivity  
5. Document findings  

---

### ⚙️ 4. Common Troubleshooting Commands

**Windows:**
ipconfig /all
ping <IP or domain>
tracert <domain>
nslookup <domain>
netstat -an

makefile
Copy code

**Linux:**
ifconfig / ip addr
ping <IP or domain>
traceroute <domain>
nslookup <domain>
netstat -an

yaml
Copy code

---

### 🗂️ 5. Practical / Lab Practice

- Ping local and external devices  
- Use `traceroute/tracert` to identify where the network fails  
- Check IP configuration and default gateway  
- Verify DNS resolution using `nslookup`  
- Test firewall rules and connectivity  

---

### 🧠 6. Key Terms

- **Ping:** Checks connectivity to a device  
- **Traceroute:** Shows path packets take to reach a destination  
- **IP Conflict:** Two devices with same IP address  
- **Bandwidth:** Maximum data transfer rate  
- **Latency:** Time taken for data to travel  

---

### 📘 Day 14 Summary

✅ Learned network troubleshooting basics  
✅ Identified common network issues  
✅ Explored troubleshooting steps and commands  
✅ Practiced testing connectivity and diagnosing problems  
