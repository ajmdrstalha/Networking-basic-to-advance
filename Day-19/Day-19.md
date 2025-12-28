## 📘 Day 19 – DNS & DHCP

### 🧩 1. What is DNS?

**DNS (Domain Name System)** translates **human-readable domain names** into **IP addresses**.

- Makes it easier to access websites (e.g., google.com → 142.250.190.78)  
- Distributed and hierarchical system  
- Works at **Application Layer**  

---

### 🔢 2. What is DHCP?

**DHCP (Dynamic Host Configuration Protocol)** automatically **assigns IP addresses and network settings** to devices.

- Reduces manual configuration  
- Assigns IP, subnet mask, gateway, and DNS server  
- Works at **Network Layer (Layer 3)**  

---

### 🔁 3. DNS Records

| Record | Description |
|--------|-------------|
| A | Maps domain to IPv4 address |
| AAAA | Maps domain to IPv6 address |
| CNAME | Alias for another domain |
| MX | Mail exchange server |
| NS | Name server for the domain |

---

### ⚙️ 4. How DNS & DHCP Work

**DNS Process:**
1. User enters a domain in browser  
2. Request sent to DNS resolver  
3. Resolver queries authoritative servers  
4. IP address returned to client  

**DHCP Process:**
1. Client sends DHCPDISCOVER broadcast  
2. DHCP server responds with DHCPOFFER  
3. Client requests IP via DHCPREQUEST  
4. Server acknowledges with DHCPACK  

---

### 🗂️ 5. Practical / Lab Practice

- Check current IP and DNS configuration:

**Windows:**
ipconfig /all
nslookup google.com

makefile
Copy code

**Linux:**
ifconfig / ip addr
dig google.com

yaml
Copy code

- Set static IP and compare with DHCP-assigned IP  
- Observe DNS resolution using `ping` and `nslookup`  
- Test DHCP lease renewal using `ipconfig /renew` or `dhclient`  

---

### 🧠 6. Key Terms

- **DNS Resolver:** Queries DNS servers to find IP  
- **Authoritative Server:** Provides official domain-IP mapping  
- **DHCP Lease:** Temporary IP assignment  
- **Scope:** Range of IPs a DHCP server can assign  
- **CNAME:** Alias mapping for domains  

---

### 📘 Day 19 Summary

✅ Learned what DNS and DHCP are  
✅ Explored DNS record types and resolution process  
✅ Understood DHCP process and IP assignment  
✅ Practiced checking and configuring DNS and DHCP settings 
