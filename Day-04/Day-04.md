## 📘 Day 4 – Default Gateway, DNS, and DHCP


### 🧩 1. Default Gateway

A **default gateway** is the router that connects a local network to external networks such as the Internet.

- Used when a device wants to communicate outside its local network  
- Usually the router’s LAN IP address  
- Without a gateway, internet access will not work  

Example:
Device IP : 192.168.1.10
Subnet Mask : 255.255.255.0
Default Gateway: 192.168.1.1

yaml
Copy code

---

### 🌍 2. Domain Name System (DNS)

DNS converts **human-readable domain names** into **IP addresses**.

Example:
www.google.com → 142.250.72.14

yaml
Copy code

Why DNS is important:
- Easy to remember domain names  
- Faster access to websites  
- Works as the phonebook of the Internet  

Common DNS Servers:
- Google DNS: `8.8.8.8`, `8.8.4.4`
- Cloudflare DNS: `1.1.1.1`
- ISP DNS

---

### 🗂️ 3. Types of DNS Records

| Record | Purpose |
|------|--------|
| A | Maps domain to IPv4 address |
| AAAA | Maps domain to IPv6 address |
| CNAME | Alias for another domain |
| MX | Mail server information |
| TXT | Verification and security data |

---

### ⚙️ 4. Dynamic Host Configuration Protocol (DHCP)

DHCP automatically assigns IP configuration to network devices.

DHCP provides:
- IP Address  
- Subnet Mask  
- Default Gateway  
- DNS Server  

Without DHCP:
- IPs must be assigned manually  
- Higher chance of IP conflicts  

---

### 🔄 5. DHCP Process (DORA)

DHCP works using the **DORA** process:

1. **Discover** – Client searches for DHCP server  
2. **Offer** – Server offers an IP address  
3. **Request** – Client requests the offered IP  
4. **Acknowledge** – Server confirms and assigns IP  

---

### 🧪 6. Practical / Lab Practice

Check network configuration:

**Windows:**
ipconfig /all

makefile
Copy code

**Linux:**
ip addr

yaml
Copy code

Test DNS resolution:
ping google.com
nslookup google.com

yaml
Copy code

---

### 🧠 7. Key Terms

- **Default Gateway:** Path to external networks  
- **DNS:** Translates domain names to IPs  
- **DHCP:** Automatically assigns IP configuration  
- **Lease Time:** Duration of assigned IP  

---

### 📘 Day 4 Summary

✅ Understood default gateway  
✅ Learned DNS and its records  
✅ Explained DHCP and DORA process  
✅ Practiced basic networking commands  

