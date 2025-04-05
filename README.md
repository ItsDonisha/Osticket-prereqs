<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine 
- Os Ticket Installtion Files
- RDP (Port 3389 Allowed on VM
- Install MYSQL
- Enabling IIS in windows vm

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/c80768ec-949f-4983-b572-33da2a367736)
1️⃣ Head to Control Panel → Programs → Turn Windows features on or off
2️⃣ Find Internet Information Services (IIS) and expand it
3️⃣ Go to World Wide Web Services → Application Development Features
4️⃣ Check the box for CGI ✅
5️⃣ Click OK, let it install, and then close out!
</p>
<br />


![image](https://github.com/user-attachments/assets/afe31971-480e-4ee5-ad99-61193eac5add)

Now that CGI is enabled, let’s get everything set up! 💻✨  

1️⃣ Install the following from the **"osTicket-Installation-Files"** folder in this order:  
   - **PHP Manager** 📂  
   - **Rewrite Module** 🔄  
   - **VC redist.x86.exe** ⚙️  
   - **MySQL file** 🛠️  

2️⃣ For **MySQL**, follow these steps:  
   - Click **Typical setup** ✅  
   - Launch **Configuration Wizard** (keep default settings)  
   - Create a **user and password** 🔑  

3️⃣ Once everything is installed, create a new directory: **C:\PHP** 📁  
4️⃣ Unzip the **PHP 7.3.8** folder inside it! 🎀💡  

And just like that, you’re one step closer to a smooth setup! 🚀💕
</p>
<br />

Next, rename the configuration file by changing ost-sampleconfig.php to ost-config.php. You can find it in **C:\inetpub\wwwroot\osTicket\include**. After renaming, assign the necessary permissions to the file. Right-click ost-config.php, select Properties, then go to the Security tab. Click Advanced, disable Inheritance, and then click Add. Select Principal, type "Everyone", and confirm by clicking OK. Next, check "Full Control", click OK, and verify the permissions under Permissions Entries to ensure the changes have been applied. 🎀💻✨
First, rename ost-sampleconfig.php to ost-config.php, located in **C:\inetpub\wwwroot\osTicket\include**. Then, update the file permissions by right-clicking ost-config.php, selecting Properties, and navigating to the Security tab. Click Advanced, disable Inheritance, and choose Add. Select Principal, enter "Everyone", and click OK. Grant Full Control, confirm with OK, and ensure the changes are applied under Permissions Entries. 🎀💻✨
![image](https://github.com/user-attachments/assets/916fbe5a-66aa-46ec-8040-a26c3f5420a0)
</p>
<br />
