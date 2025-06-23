# Nmap-Scanning-Local-IP
Using **Nmap** to Scan Local Ip and all available ports for scanning of the system

Use the Following Command to install Nmap on Kali Linux in the Terminal:
Code
```
 sudo apt-install Nmap 
 ```


Step 1: Find Your Local IP address:
Find Local IP using the following Command on your Terminal/Command Prompt:

On Windows:
Code
```
ipconfig
```
On Mac/Linux:
Code
```
ifconfig
```
Look for an IPv4 address like 192.168.1.x. Your scan range will typically be 192.168.1.0/24.


**🔎 Step 2: Discover Active Devices**

Use a ping scan to detect active devices on the network:
```
nmap -sn [IP address]
```
Replace [IP address] with your Local IP address

**Step 3: To scan The Network and Store the Output in a Textfile, we would write command:**
Code
```
nmap -sS -p- [IP address]/[subnet] -oN fullScanning.txt
```
**-sS : TCP SYN scan (stealthy and efficient)
-p- : Scan all 65,535 TCP ports
-oN : Save output in normal text format***



**📁 After the Scan**
Once the scan is complete, open the fullScanning.txt file to view open ports and detected hosts/services in your local network.
