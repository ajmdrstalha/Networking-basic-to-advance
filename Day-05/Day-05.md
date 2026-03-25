## 📘 Day 5 – MAC Address & ARP (Address Resolution Protocol)

### 🧩 1. What is a MAC Address?

A **MAC (Media Access Control) address** is a **unique physical address** assigned to a network interface card (NIC).

- Fixed by the manufacturer  
- Works at **Layer 2 (Data Link Layer)**  
- Used for communication inside a LAN  

Example:
00:1A:2B:3C:4D:5E

yaml
Copy code

---

### 🔢 2. MAC Address Structure

A MAC address is **48 bits (6 bytes)** long.

Format:
XX:XX:XX:XX:XX:XX

yaml
Copy code

| Part | Meaning |
|------|--------|
| First 3 bytes | OUI (Organization Unique Identifier) |
| Last 3 bytes | Device unique number |

---

### 🔁 3. What is ARP?

ARP (Address Resolution Protocol) is used to **map an IP address to a MAC address** inside a local network.

Example:
IP Address → MAC Address
192.168.1.1 → 00:1A:2B:3C:4D:5E


---

### ⚙️ 4. How ARP Works

1. Device sends ARP request (broadcast)  
2. Target device replies with its MAC address  
3. Sender stores MAC in ARP table  
4. Communication continues using MAC address  

---

### 🗂️ 5. ARP Table

The ARP table stores **IP-to-MAC mappings**.

Check ARP table:

**Windows:**
arp -a

makefile
Copy code

**Linux:**
ip neigh

yaml
Copy code

---

### ⚠️ 6. ARP Issues & Security

- ARP spoofing / poisoning  
- Man-in-the-middle attacks  
- Can be prevented using static ARP entries or security tools  

---

### 🧪 7. Practical / Lab Practice

- Run `arp -a` before and after pinging another device  
- Observe how MAC addresses are learned  
- Clear ARP cache and test again  

---

### 🧠 8. Key Terms

- **MAC Address:** Physical address of NIC  
- **ARP:** Resolves IP to MAC  
- **Broadcast:** Sent to all devices in LAN  
- **Unicast:** Sent to a single device  

---

### 📘 Day 5 Summary

✅ Learned MAC address basics  
✅ Understood ARP and its working  
✅ Explored ARP table and commands  
✅ Identified ARP security issues  

