# Task1-Elevate-Labs
1. First i installed nmap with sudo apt install nmap
2. then i used ifconfig to check my ip address for eth0 vmware machine which was inet 192.X.X.X
3. I ran the command of nmap Tcp Syn scan which was sudo (because i was not root user here) nmap -sS ip address -oN(write it to a file) task1.txt
4. You can see the task1.txt scan results as for my vmware i found my port 53/tcp open
5. port 53 is usually used for running dns services and is vulnerable to dns amplification attacks
6. After the nmap i i openend by wireshark which required me to enter the user password to launch
7. As in my wireshark folder i have attached images of my results
8. i started my eth0 interface which will start analyzing it on my ip address
9. In img1 i started wireshark and in img2 my interface has just started and is not receiving any packets because i have not yet started my browser
10. by starting my firefox browser in kali i have initiated it to start capturing the packets which are going in and on from my computer
11. img3 justifies the packet analyzing
    
