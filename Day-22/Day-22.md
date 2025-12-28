## 📘 Day 22 – Introduction to SDN (Software-Defined Networking)

### 🧩 1. What is SDN?

**SDN (Software-Defined Networking)** is a network architecture approach that **separates the control plane from the data plane**.

- Centralized control of network devices  
- Enables automation, programmability, and flexibility  
- Reduces complexity in managing large networks  

Example:
- Central controller manages multiple switches and routers  
- Network policies can be updated without touching individual devices  

---

### 🔢 2. Key Components of SDN

| Component | Description |
|-----------|-------------|
| Controller | Centralized software managing the network |
| Switch / Router | Data plane devices forwarding traffic |
| Southbound API | Interface between controller and network devices (e.g., OpenFlow) |
| Northbound API | Interface between controller and applications/services |

---

### 🔁 3. Benefits of SDN

- Simplified network management  
- Dynamic and automated configuration  
- Enhanced security and segmentation  
- Better traffic monitoring and analytics  
- Rapid deployment of new services  

---

### ⚙️ 4. How SDN Works

1. Network devices forward packets based on controller instructions  
2. Controller collects real-time network information  
3. Policies and routing rules are programmed centrally  
4. Devices update forwarding tables dynamically  

---

### 🗂️ 5. Practical / Lab Practice

- Explore an SDN controller like **OpenDaylight** or **Cisco APIC**  
- Connect virtual switches to the controller  
- Create a simple flow rule to allow or block traffic  
- Observe how changes in the controller propagate to switches  
- Monitor traffic and verify flow rules in real-time  

---

### 🧠 6. Key Terms

- **Control Plane:** Part of network that decides where traffic is sent  
- **Data Plane:** Part of network that forwards traffic based on rules  
- **Controller:** Central software managing network behavior  
- **OpenFlow:** Protocol used for communication between controller and devices  
- **Flow Table:** Rules installed on switches to forward traffic  

---

### 📘 Day 22 Summary

✅ Learned what SDN is and its architecture  
✅ Explored SDN components and APIs  
✅ Understood the benefits of centralized network control  
✅ Practiced basic SDN flow rules and monitoring  
