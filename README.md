🚫 Step 1: Disable Antivirus (Windows Defender)

Cain & Abel is often detected as a hacking tool by antivirus software.

Open Windows Security

Go to Virus & Threat Protection

Temporarily disable Real-Time Protection

📥 Step 2: Download Required Software

Download the following two tools:

Cain & Abel

WinPcap

Make sure you download both before starting the installation.

🧩 Step 3: Install WinPcap (First)

Run the WinPcap installer

Complete the installation using default settings

✅ WinPcap must be installed before Cain & Abel.

🧪 Step 4: Install Cain & Abel

Run the Cain & Abel installer

When Windows shows a warning, click Run anyway

During installation, it may ask to install WinPcap again

Click Don’t install (because it is already installed)

🌐 Step 5: Configure Network Adapter Settings

Open Control Panel

Go to
Network and Internet → Network and Sharing Center

Click Change adapter settings

Right-click on the network adapter you are using
(example: Ethernet 0) → Properties

🔹 Disable IPv6

Uncheck Internet Protocol Version 6 (IPv6)

🔹 Configure IPv4

Select Internet Protocol Version 4 (IPv4)

Click Properties

Click Advanced

Go to the DNS tab

Make sure both checkboxes are ticked

Click OK

Close all settings windows

🖥️ Step 6: Disable Task Offloading (Required)

Open PowerShell as Administrator

Run the following command:

netsh int ip set global taskoffload=disable


Press Enter

✅ Final Notes

Restart your system if required

Always run Cain & Abel as Administrator
