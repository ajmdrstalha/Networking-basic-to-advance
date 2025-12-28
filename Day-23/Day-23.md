## 📘 Day 23 – Network Virtualization & Overlay Networks

### 🧩 1. What is Network Virtualization?

**Network Virtualization** is the process of **abstracting physical network resources** to create multiple virtual networks.

- Each virtual network can have its own topology, policies, and services  
- Provides flexibility, isolation, and efficient resource utilization  
- Works with SDN and cloud environments  

Example:
- Multiple tenants using the same physical network infrastructure in a data center  

---

### 🔢 2. Types of Network Virtualization

| Type | Description |
|------|-------------|
| VLAN | Divides a physical LAN into multiple logical networks |
| VXLAN | Encapsulates Layer 2 frames over Layer 3 networks |
| NVGRE | Network Virtualization using Generic Routing Encapsulation |
| VRF | Virtual Routing and Forwarding, isolates routing tables |

---

### 🔁 3. Overlay Networks

**Overlay Networks** are virtual networks built **on top of physical networks**.

- Uses encapsulation to tunnel traffic  
- Allows independent network topology and policies  
- Common in cloud and data center networks  

Example:
- VXLAN creates an overlay network over existing IP infrastructure  

---

### ⚙️ 4. How Network Virtualization Works

1. Physical network provides connectivity and bandwidth  
2. Virtual networks are created using VLANs, VXLANs, or VRFs  
3. Overlay protocols encapsulate traffic for isolation  
4. Virtual network management tools control and monitor traffic  

---

### 🗂️ 5. Practical / Lab Practice

- Create multiple VLANs on a managed switch  
- Configure VXLAN in a virtual lab environment  
- Test communication between virtual networks  
- Observe traffic encapsulation and routing  
- Monitor virtual network performance using tools  

---

### 🧠 6. Key Terms

- **Virtual Network:** Logical network created over physical infrastructure  
- **Overlay Network:** Encapsulated network on top of physical network  
- **VXLAN:** Encapsulates Layer 2 traffic over Layer 3 network  
- **VRF:** Isolated routing table for multiple virtual networks  
- **Network Segmentation:** Dividing network into isolated parts  

---

### 📘 Day 23 Summary

✅ Learned what network virtualization is  
✅ Explored VLAN, VXLAN, NVGRE, and VRF  
✅ Understood overlay networks and encapsulation  
✅ Practiced creating and monitoring virtual networks
