# SkyTower: Vulnerable Web Server 🏰  
![SkyTower Logo](logo.png)

**SkyTower** is a deliberately vulnerable web server environment built on **Alpine Linux** using **Docker**.  
It integrates **OWASP WebGoat** and **WebWolf** to provide a lightweight, easily configurable lab for practicing web application security.  

---

## 🔹 Features
- Built on **Alpine Linux** (lightweight, VM‑friendly).  
- Runs **WebGoat** and **WebWolf** inside Docker containers.  
- Preconfigured to expose vulnerabilities for training (SQLi, XSS, CSRF, insecure configs, etc.).  
- Accessible via **host browser** (with VirtualBox networking).  
- Supports testing with **OWASP ZAP, Burp Suite, and custom scripts**.  

---

## 🔹 Default Credentials  

### 🖥️ System Access  
- **Root User**:  
  - Username: `root`  
  - Password: `211009988`  

- **Agent User** (non‑privileged):  
  - Username: `agent`  
  - Password: `211009988`  

*(⚠️ These are intentionally weak credentials for training purposes — do not use in production!)*  
 

---

## 🔹 Setup Instructions  

### 1️⃣ Import SkyTower VM into VirtualBox  
1. Download the **SkyTower.ova** file.  
2. Open **VirtualBox** → Go to **File > Import Appliance**.  
3. Select the `SkyTower.ova` file and click **Next** → **Import**.  
4. After import, you will see the **SkyTower VM** in your VirtualBox list.  

---

### 2️⃣ Start the VM  
1. Select **SkyTower VM** and click **Start**.  
2. Log in with the default credentials:  
   - **Root User:** `root / 211009988`  
   - **Agent User:** `agent / 211009988`  

---

### 4️⃣ Accessing Applications  
- **WebGoat:**  
  - `http://<vm-ip>:8080/WebGoat` (Bridged mode)  

- **WebWolf:**    
  - `http://<vm-ip>:9090/WebWolf` (Bridged mode)  

---



