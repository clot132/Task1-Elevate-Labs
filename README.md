Task 1: Scan Your Local Network for Open Ports
Objective: Learn to discover open ports on devices in your local network to understand network exposure.
Tools: Nmap (free), Wireshark (optional)

1. Installed Nmap using the command:
      sudo apt install nmap

2. Found the IP address of my local machine (VMware eth0 interface) using:
      ifconfig

      Identified the local IP as: 192.X.X.X

3. Ran a TCP SYN scan on my own IP address using the following command (as a non-root user):
      sudo nmap -sS 192.X.X.X -oN task1.txt

      This saved the scan results to task1.txt.

4. From the Nmap results, observed that only port 53/tcp was open.

      Port 53 is used for DNS (Domain Name System) services.

      It can be vulnerable to DNS amplification attacks if misconfigured or exposed.

5.Opened Wireshark to analyze live packet traffic.

 Required entering the user password to launch the tool.

6. Started packet capture on the eth0 interface in Wireshark.

      img1.png: Wireshark launched

      img2.png: Interface started, no packets received (browser not yet opened)

      img3.png: Firefox browser started, showing captured network packets

7. Observed real-time network traffic using Wireshark to understand how browsing activity generates and sends packets.

8. Scan results were saved in the task1.txt file for documentation and further analysis.

Security Risk Summary


The following port was found open and may pose a security risk:

Port	Service	Risk
53	DNS	Can be abused for amplification attacks



Files Included

nmap/task1.txt – Nmap scan result file

Inside Wireshark Folder---

img1.png, img2.png, img3.png – Wireshark screenshots

README.md – This documentation

