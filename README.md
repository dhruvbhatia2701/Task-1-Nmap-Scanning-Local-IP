# Task-1-Nmap-Scanning-Local-IP
Using Nmap to Scan Local Ip and all available ports for scanning of the system

Use the Following Command to install Nmap on Kali Linux in the Terminal:
Code
```
 sudo apt-install Nmap 
 ```
Find Local IP using the following Command on your Terminal/Command Prompt:

On Windows:

Code```
ipconfig```

On Mac/Linux:

Code```
ifconfig```

To scan The Network , we would write command:
Code```
nmap -sS -p- [IP address]/[subnet]```
