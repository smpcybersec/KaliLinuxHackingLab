<h1>Kali Linux Hacking Lab - WIP</h1>

<h2>Description</h2>

Step-by-step process of virtualizing, installing, and setting up a Kali Linux virtual machine to carry out network scans and exploitations of an emulated corporate network with the goal of documenting attacks from the Kali machine and incident response from the emulated corporate network.

<sub><b>**This repository assumes familiarization with virtualization software</b></sub>
<br />
<br />
<p align="center">
<b>[Virtualization and Installing Kali Linux]</b>
<br />
<br />
<img src="https://i.imgur.com/mKYRKWQ.png" width="50%" height="50%">
<br />
<sub>From VirtualBox Manager, select "New"</sub>
<br />
<br />
<img src="https://i.imgur.com/TVrXCUs.png" width="50%" height="50%">
<br />
<sub>Name virtual machine
<br />
Load Kali Linux ISO image
<br />
Click "Next"</sub>
<br />
<br />
<img src="https://i.imgur.com/ber0oZF.png" width="50%" height="50%">
<br />
<sub>Finish setting up virtual machine with memory, processors, and storage
<br />
On VirtualBox Manager, click "Settings" for Kali Linux machine</sub>
<br />
<br />
<img src="https://i.imgur.com/V1s8byY.png" width="50%" height="50%">
<br />
<sub>Click "Disk Encryption" tab on General Settings
<br />
Enter disk encryption password
<br />
Click "OK"</sub>
<br />
<br />
<img src="https://i.imgur.com/uTUlwwU.png" width="50%" height="50%">
<br />
<sub>Start up Kali Linux machine
<br />
Select "Graphical install" when prompted</sub>
<br />
<br />
<img src="https://i.imgur.com/l9mutpL.png" width="50%" height="50%">
<br />
<sub>Enter disk encryption password
<br />
Click "OK"</sub>
<br />
<br />
<img src="https://i.imgur.com/014AOdQ.png" width="50%" height="50%">
<br />
<sub>Select language, location, and keyboard layout
<br />
Continue to installation</sub>
<br />
<br />
<img src="https://i.imgur.com/ax4FRzt.png" width="50%" height="50%">
<br />
<sub>When prompted, enter a hostname for machine
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/Gywrl57.png" width="50%" height="50%">
<br />
<sub>Enter domain name
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/4iiuS60.png" width="50%" height="50%">
<br />
<sub>Enter name of user
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/Cp51jD5.png" width="50%" height="50%">
<br />
<sub>Enter desired username
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/j9mTiEI.png" width="50%" height="50%">
<br />
<sub>Enter and re-enter password
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/9QBkpwz.png" width="50%" height="50%">
<br />
<sub>Select time zone
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/Hn0Npo4.png" width="50%" height="50%">
<br />
<sub>Select "Guided - use entire disk" to partition entire allocated disk space to operating system
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/GmtWTA6.png" width="50%" height="50%">
<br />
<sub>Only one option appears in disk partitioning
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/iPSiR3t.png" width="50%" height="50%">
<br />
<sub>By default, "All files in one partition" is selected
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/x3seDrY.png" width="50%" height="50%">
<br />
<sub>Finish disk partitioning
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/18EK0nh.png" width="50%" height="50%">
<br />
<sub>Confirm writing changes to disk
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/fatE0cB.png" width="50%" height="50%">
<br />
<sub>Let installation run until you are prompted for software selection</sub>
<br />
<br />
<img src="https://i.imgur.com/B95qm9q.png" width="50%" height="50%">
<br />
<sub>For now, the default selections for software are enough for current use case
<br />
Click "Continue"
</sub>
<br />
<br />
<img src="https://i.imgur.com/zag5Vov.png" width="50%" height="50%">
<br />
<sub>Allow installation to run until prompted to install GRUB boot loader</sub>
<br />
<br />
<img src="https://i.imgur.com/BLD2R3J.png" width="50%" height="50%">
<br />
<sub>Select "Yes" to install GRUB boot loader to primary drive
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/vMPrUJw.png" width="50%" height="50%">
<br />
<sub>Highlight the device that appears beginning with "/dev/sda"
<br />
Click "Continue"</sub>
<br />
<br />
<img src="https://i.imgur.com/dppkYZk.png" width="50%" height="50%">
<br />
<sub>Allow installation of Kali Linux to finish
<br />
Select "Continue" to reboot the machine</sub>
<br />
<br />
<img src="https://i.imgur.com/odIXiF4.png" width="50%" height="50%">
<br />
<sub>Log in using username and password created during installation</sub>
<br />
<br />
<b>[Kali Linux Initial Setup]</b>
<br />
<br />
<img src="https://i.imgur.com/edlcOqv.png" width="50%" height="50%">
<br />
<sub>Upon logging in, open Terminal Emulator on toolbar at top of screen
<br />
**Alternatively, pressing Ctrl-Alt-T opens Terminal Emulator
<br />
Enter command:</sub>
  
  ```
  sudo apt update && sudo apt upgrade -y
  ```
</p>

<p align="center">
<sub>**This updates and upgrades all installed packages using sudo privileges and auto-confirms upgrades</sub>
<br />
<br />
<img src="https://i.imgur.com/MLciwJ7.png" width="50%" height="50%">
<br />
<sub>After entering sudo (root) password, wait for updates and upgrades to finish.</sub>
<br />
<br />
<img src="https://i.imgur.com/ytPCZet.png" width="50%" height="50%">
<br />
<sub>Enter command:</sub>

  ```
  sudo apt autoremove -y
  ```

</p>
  
<p align="center">
<sub>**This removes packages deemed no longer necessary for dependencies
<br />
Enter sudo password</sub>
<br />
<br />
<img src="https://i.imgur.com/7JSFQJZ.png" width="50%" height="50%">
<br />
<sub>Wait for autoremove to finish
<br />
Take snapshot of current machine state</sub>
<br />
<br />
<b>[Taking A Snapshot of A Virtual Machine]</b>
<br />
<br />
<img src="https://i.imgur.com/pDTh37R.png" width="50%" height="50%">
<br />
<sub>Click "Machine" on toolbar at top left of virtual machine window
<br />
Select "Take Snapshot..."</sub>
<br />
<br />
<img src="https://i.imgur.com/m8GDiAr.png" width="50%" height="50%">
<br />
<sub>Name and describe snapshot
<br />
**I name mine by date and time taken and describe the snapshot as what changes to the machine I have made.</sub>
<br />
<br />
<b>[Tools of the Trade]</b>
<br />
<br />
<img src="https://i.imgur.com/qh2ubOf.png" width="50%" height="50%">
<br />
<sub>Ensuring nmap is installed using:</sub>
</p>

  ```
  nmap --version
  ```

<p align="center">
<sub>nmap is used to scan and enumerate networks.  It can be configured to run scans at various speeds and with different obfuscation methods to avoid detection.
<br />
It is a powerful tool for both Red Team and Blue Team.</sub>
<br />
<br />
<img src="https://i.imgur.com/uTLtU5Z.png" width="50%" height="50%">
<br />
<sub>Ensuring Metasploit framework is installed using:</sub>
</p>

  ```
  msfconsole --version
  ```

<p align="center">
<sub>The Metasploit framework is a tool used by ethical hackers and malicious actors to probe systems for vulnerabilities and exploits them.
<br />
Being an open-source framework, it can be customized and appended.</sub>
<br />
<br />
<img src="https://i.imgur.com/FNse4hF.png" width="50%" height="50%">
<br />
<sub>Ensuring Python3 is installed using:</sub>
</p>

  ```
  python3 --version
  ```

<p align="center">
<sub>Python is a programming language popular with hackers because of its simplicity in its syntax.
<br />
Python is also open-source, cross-platform, extendable with low-level modules, and has a broad standard library.</sub>
<br />
<br />
<img src="https://i.imgur.com/LqGLNEC.png" width="50%" height="50%">
<br />
<sub>Ensuring Git is installed using:</sub>
</p>

  ```
  git --version
  ```

<p align="center">
<sub>Git is used for version control in tracking updates to a file, or checking integrity of a file.</sub>
<br />
<br />
<img src="https://i.imgur.com/B5fKrwV.png" width="50%" height="50%">
<br />
<sub>By default, Kali Linux will not have VSCode, or code-oss, installed.
<br />
Install VSCode/code-oss using:</sub>
</p>

  ```
  sudo apt install code-oss
  ```

<p align="center">
<b>[Changing Root Account Password]</b>
<br />
<br />
<img src="https://i.imgur.com/l7YHa6l.png" width="50%" height="50%">
<br />
<sub>It is bad practice to use default credentials.  Changing the root password is imperative.
<br />
Enter the command:</sub>
</p>

  ```
  sudo su
  ```

<p align="center">
<sub>**You may have to enter your sudo password
<br />
From the root account, change the root account password</sub>
<br />
<br />
<img src="https://i.imgur.com/r4qqKYg.png" width="50%" height="50%">
<br />
<sub>Enter the command:</sub>
</p>

  ```
  passwd
  ```

<p align="center">
<sub>Enter and re-enter secure password</sub>
<br />
<br />
<b>[Creating a Low-Level User]</b>
<br />
<br />
<img src="https://i.imgur.com/T2H89tI.png" width="50%" height="50%">
<br />
<sub>Creating a low-level user to use as a main account is best practice.
<br />
With future updates on user permissions, this ensures only trusted accounts have sudo (root) priveleges.
<br />
From the root account, enter the command:</sub>
</p>

  ```
  adduser <username>
  ```

<p align="center">
<sub>A new user account is added to your kernel's user directories</sub>
<br />
<br />
<img src="https://i.imgur.com/jI838fP.png" width="50%" height="50%">
<br />
<sub>Enter new account's password.</sub>
<br />
<br />
<img src="https://i.imgur.com/b7M1RZM.png" width="50%" height="50%">
<br />
<sub>Continue pressing Enter until prompted "Is this information correct?"
<br />
Enter "Y"
<br />
Press Enter</sub>
<br />
<br />
<b>[Adding sudoer Privileges to User Accounts]</b>
<br />
<br />
<img src="https://i.imgur.com/OdIgTRb.png" width="50%" height="50%">
<br />
<sub>From the root account, enter the command:</sub>
</p>

  ```
  usermod -aG sudo <username>
  ```

<p align="center">
<sub>**The argument "-aG" is appending (a) to the sudo group (G)</sub>
<br />
<br />
<img src="https://i.imgur.com/iBJzJVs.png" width="50%" height="50%">
<br />
<sub>Change the user's login shell to bash using the command:</sub>
</p>

  ```
  chsh -s /bin/bash <username>
  ```

<p align="center">
<sub>This change's the new user's default shell to bash, the shell currently in use for terminal commands.</sub>
<br />
<br />
<img src="https://i.imgur.com/3eFX1Ks.png" width="50%" height="50%">
<br />
<sub>Switch to new low-level user using the command:</sub>
</p>

  ```
  su <username>
  ```

<p align="center">
<br />
<br />
<b>[Installing A Multiplexer]</b>
<br />
<br />
<img src="https://i.imgur.com/e0Z9Che.png" width="50%" height="50%">
<br />
<sub>From new user account, enter command:</sub>
</p>

  ```
  sudo apt install konsole -y
  ```

<p align="center">
<sub>Enter sudo password.
<br />
**Konsole is a multiplexer used to operate from multiple terminals simultaneously.
<br />
**Tilix can also be used as well as Guake.</sub>
<br />
<br />
<img src="https://i.imgur.com/ylVt7Yk.png" width="50%" height="50%">
<br />
<sub>Open Konsole by typing the following command:</sub>
</p>

  ```
  sudo konsole
  ```

<p align="center">
<br />
<br />
<img src="https://i.imgur.com/ylVt7Yk.png" width="50%" height="50%">
<br />
<sub>Split the terminal either horizontally or vertically by selecting from the "Split View" dropdown menu at the top of the Konsole toolbar.</sub>
<br />
<br />
<b>[Installing and Setting Up A VPN]</b>
<br />
<br />
<img src="https://i.imgur.com/MkFmTAM.png" width="50%" height="50%">
<br />
<sub>Using NordVPN, per NordVPN's website on installing and configuring on Linux:
<br />
To download via command line, enter the following command:</sub>
</p>

  ```
  sh <(curl -sSf https://downloads.nordcdn.com/apps/linux/install.sh
  ```

<p align="center">
<sub>Enter sudo password to continue download.
<br />
**This command downloads and installs the NordVPN client for Linux</sub>
<br />
<br />
<img src="https://i.imgur.com/t4DBIUd.png" width="50%" height="50%">
<br />
<sub>Wait for prompt to continue with installation.
<br />
Press "Y"
<br />
Press Enter</sub>
<br />
<br />
<img src="https://i.imgur.com/NylRq50.png" width="50%" height="50%">
<br />
<sub>One more step to make sure NordVPN can be used by this user is to enter the following command:</sub>
</p>

  ``` 
  sudo usermod -aG nordvpn $USER
  ```

<p align="center">
<sub>This will allow the current $USER to use NordVPN client via command line interface</sub>
<br />
<br />
<img src="https://i.imgur.com/AE6DXeQ.png" width="50%" height="50%">
<br />
<sub>Reboot machine to apply adding current $USER to nordvpn group using:</sub>
</p>

  ```
  sudo reboot
  ```

<p align="center">
<br />
<br />
<img src="https://i.imgur.com/Ee9syHk.png" width="50%" height="50%">
<br />
<sub>Upon reboot, open terminal emulator and enter the following command:</sub>
</p>

  ```
  nordvpn set technology openvpn
  ```

<p align="center">
<sub>OpenVPN is a stable, secure, and open-source VPN protocol that supports both TCP and UDP protocols.
<br />
NordLynx is also an option, but I have grown to rely on OpenVPN's stability.  NordLynx may be faster for others.</sub>
<br />
<br />
<img src="https://i.imgur.com/s1GjESN.png" width="50%" height="50%">
<br />
<sub>Another technology I enable from the start is Threat Protection Lite.  To do this, enter the command:</sub>
</p>

  ```
  nordvpn set threatprotectionlite on
  ```

<p align="center">
<sub>Threat Protection Lite is a feature that blocks ads, trackers, and malicious URLs while getting rid of downloaded malware.</sub>
<br />
<br />
<b>[Logging Into NordVPN]</b>
<br />
<br />
<img src="https://i.imgur.com/XPi2fZK.png" width="50%" height="50%">
<br />
<sub>To log into NordVPN via command line, enter the command:</sub>
</p>

  ```
  nordvpn login
  ```

<p align="center">
<sub>This will prompt an external link to visit in order to be able to sign into the client via command line.</sub>
<br />
<br />
<img src="https://i.imgur.com/2URoi8F.png" width="50%" height="50%">
<br />
<sub>Right-click link in terminal emulator
<br />
Click "Open Link"
<br />
This will open a browser tab, taking you to NordVPN's login page on their website</sub>
<br />
<br />
<img src="https://i.imgur.com/tjDTHzS.png" width="50%" height="50%">
<br />
<sub>Log in using credentials</sub>
<br />
<br />
<img src="https://i.imgur.com/WX1KfsV.png" width="50%" height="50%">
<br />
<sub>After verifying being logged in, connect to VPN using the command:</sub>
</p>

  ```
  nordvpn connect
  ```

<p align="center">
<sub>The Kali Linux machine is now set up and ready to begin carrying out network scans and attacks.</sub>
<br />
<br />
</p>
