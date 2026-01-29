# Cain and Abel + WinPcap Setup Guide (Windows)

This repository provides a **step-by-step guide** to correctly install and configure **Cain and Abel** with **WinPcap** on Windows systems.  
Follow the instructions carefully to avoid common installation and network issues.

## Installation Steps

### 1️⃣ Disable Antivirus (Windows Defender)
Temporarily disable Windows Defender or any other antivirus software to prevent installation issues.

---

### 2️⃣ Download Required Software
Download **both** of the following:
- Cain and Abel
https://web.archive.org/web/20160311154514/http://www.oxid.it/downloads/ca_setup.exe
- 
- WinPcap
- https://www.winpcap.org/install/

---

### 3️⃣ Install WinPcap
- Run the **WinPcap installer**
- Complete the installation normally

---

### 4️⃣ Install Cain and Abel
- Run the **Cain and Abel installer**
- Click **Run anyway** if Windows shows a warning
- When prompted to install WinPcap again:
  - Click **Don’t Install** (because it is already installed)

---

## Network Configuration

### 5️⃣ Modify Network Adapter Settings

Go to:
Control Panel
→ Network and Internet
→ Network and Sharing Center
→ Change adapter settings


Then:

1. Right-click the network adapter you are using  
   (e.g. **Ethernet 0** or **Wi-Fi**)
2. Click **Properties**
3. **Disable IPv6**
4. Select **Internet Protocol Version 4 (IPv4)** → **Properties**
5. Click **Advanced**
6. Go to the **DNS** tab
7. Make sure **both checkboxes are ticked**
8. Click **OK** and close all settings

---

## PowerShell Configuration

### 6️⃣ Disable Task Offloading

1. Open **PowerShell as Administrator**
2. Run the following command **exactly as shown**:

3. netsh int ip set global taskoffload=disable

4. Press **Enter**

---

## Final Notes

- Restart your system after completing all steps
- Ensure you are running Cain and Abel with **administrator privileges**
- If network sniffing does not work, re-check:
  - WinPcap installation
  - IPv4 DNS settings
  - Antivirus status

---

