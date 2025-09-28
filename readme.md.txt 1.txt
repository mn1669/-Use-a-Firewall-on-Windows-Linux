Setup and Use a Firewall on Windows/Linux

## 📌 Objective
The goal of this task is to configure and test basic firewall rules to **allow or block traffic** on specific ports.  
This demonstrates how firewalls filter network traffic and improve security.

---

## 🛠 Tools Used
- **Windows Firewall with Advanced Security** (Windows 10/11)  
- **UFW (Uncomplicated Firewall)** (Linux - Ubuntu/Debian)  
- **OpenSSH Server** (for testing allowed port 22)  
- **Telnet / Netcat (nc)** (for testing connections)

---

## 🔹 Steps Performed

### 1️⃣ List Current Firewall Rules
- On **Windows**: Open `wf.msc` → Inbound Rules.  
- On **Linux**: Run `sudo ufw status`.  

📸 *[Insert screenshot of initial firewall rules]*

---

### 2️⃣ Block Port 23 (Telnet)
- **Windows**: Created a new inbound rule to **block TCP port 23**.  
- **Linux**:  
  ```bash
  sudo ufw deny 23/tcp
  sudo ufw status
