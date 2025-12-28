## 📘 Day 25 – Network Access Control (NAC)

### 🧩 1. What is NAC?

**Network Access Control (NAC)** is a security approach that **controls device access to a network based on compliance policies**.

- Ensures only authorized and compliant devices connect  
- Protects against malware, unauthorized access, and insider threats  
- Works with switches, routers, firewalls, and endpoint agents  

Example:
- Only devices with updated antivirus and patches can access the network  

---

### 🔢 2. NAC Components

| Component | Description |
|-----------|-------------|
| Policy Server | Central system defining access rules |
| Enforcement Point | Device (switch/router/AP) that enforces access policies |
| Endpoint | Device trying to access the network |
| Agent | Software on endpoints reporting compliance status |

---

### 🔁 3. NAC Modes

| Mode | Description |
|------|-------------|
| Inline | NAC device sits in the path of traffic and actively controls access |
| Out-of-Band | NAC device monitors traffic and instructs enforcement devices |
| Agent-Based | Endpoint software communicates compliance with NAC server |
| Agentless | Device access verified without software agent, using profiling |

---

### ⚙️ 4. How NAC Works

1. Endpoint requests network access  
2. NAC checks device identity and compliance  
3. Device allowed, quarantined, or denied based on policy  
4. Continuous monitoring ensures compliance  

---

### 🗂️ 5. Practical / Lab Practice

- Deploy a NAC solution in a test environment (Cisco ISE or FreeNAC)  
- Connect compliant and non-compliant devices  
- Observe enforcement actions (allow/quarantine/deny)  
- Modify policies and test changes in access behavior  
- Monitor logs for NAC events  

---

### 🧠 6. Key Terms

- **Endpoint:** Device attempting network access  
- **Policy Server:** Defines access rules and compliance criteria  
- **Quarantine:** Restricted access for non-compliant devices  
- **Inline/Out-of-Band:** NAC deployment modes  
- **Compliance:** Meeting security requirements to gain access  

---

### 📘 Day 25 Summary

✅ Learned what NAC is and why it’s important  
✅ Explored NAC components and modes  
✅ Understood how NAC enforces network security  
✅ Practiced deploying NAC and monitoring access control 
