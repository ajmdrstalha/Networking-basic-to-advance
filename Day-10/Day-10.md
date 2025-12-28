## 📘 Day 10 – NAT & PAT

### 🧩 1. What is NAT?

**NAT (Network Address Translation)** is a method to **map private IP addresses to public IP addresses** for communication over the Internet.

- Hides internal network structure  
- Conserves public IP addresses  
- Works at **Layer 3 (Network Layer)**  

Example:
Private IP: 192.168.1.10 → Public IP: 203.0.113.5

yaml
Copy code

---

### 🔢 2. Types of NAT

| Type | Description |
|------|-------------|
| Static NAT | One-to-one mapping of private to public IP |
| Dynamic NAT | Maps private IPs to a pool of public IPs |
| PAT (Port Address Translation) | Maps multiple private IPs to one public IP using different ports |

---

### 🔁 3. What is PAT?

**PAT (Port Address Translation)**, also called **NAT overload**, allows **many devices to share a single public IP**.

- Uses TCP/UDP port numbers to differentiate connections  
- Common in home networks and small offices  

Example:
192.168.1.10:5000 → 203.0.113.5:10000
192.168.1.11:5001 → 203.0.113.5:10001

yaml
Copy code

---

### ⚙️ 4. How NAT & PAT Work

1. Device sends packet with private IP  
2. NAT device replaces private IP with public IP  
3. Stores mapping in translation table  
4. Receives return traffic and translates back to private IP  

---

### 🗂️ 5. Practical / Lab Practice

- View NAT translations on routers:

**Cisco CLI:**
show ip nat translations

cpp
Copy code

- Configure static NAT:
ip nat inside source static 192.168.1.10 203.0.113.5

diff
Copy code

- Configure PAT:
ip nat inside source list 1 interface Gig0/0 overload

yaml
Copy code

---

### 🧠 6. Key Terms

- **NAT:** Translates private IP to public IP  
- **PAT:** Multiple private IPs share one public IP  
- **Inside Local:** Private IP of internal host  
- **Inside Global:** Public IP assigned by NAT  
- **Translation Table:** Stores active NAT mappings  

---

### 📘 Day 10 Summary

✅ Learned NAT and its types  
✅ Understood PAT (NAT overload)  
✅ Explored NAT translation process  
✅ Practiced NAT and PAT configuration  
