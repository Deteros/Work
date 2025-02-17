Here's a Markdown-formatted list of network troubleshooting commands for both Windows and Linux:  

```md
# Network Troubleshooting Commands for Windows and Linux

## Windows Commands

### 1. Check Network Configuration
```powershell
ipconfig /all
```
Displays detailed network configuration, including IP address, gateway, and DNS settings.

### 2. Release and Renew IP Address
```powershell
ipconfig /release
ipconfig /renew
```
Releases and renews the IP address assigned by DHCP.

### 3. Flush DNS Cache
```powershell
ipconfig /flushdns
```
Clears the DNS cache to resolve potential domain resolution issues.

### 4. Test Connectivity (Ping)
```powershell
ping google.com
```
Sends ICMP echo requests to test network connectivity.

### 5. Trace Network Path
```powershell
tracert google.com
```
Traces the route packets take to a destination.

### 6. Check Open Ports
```powershell
netstat -ano
```
Displays active connections and listening ports with process IDs.

### 7. Test DNS Resolution
```powershell
nslookup google.com
```
Resolves a domain name to an IP address using DNS.

### 8. Check Network Interface Status
```powershell
netsh interface show interface
```
Lists all network interfaces and their statuses.

### 9. Reset TCP/IP Stack
```powershell
netsh int ip reset
```
Resets the TCP/IP stack to its default state.

### 10. Display Routing Table
```powershell
route print
```
Shows the system's routing table.

---

## Linux Commands

### 1. Check Network Configuration
```bash
ip a
```
Displays IP addresses and interface information.

### 2. Check Network Connectivity (Ping)
```bash
ping -c 4 google.com
```
Sends ICMP echo requests to test connectivity.

### 3. Trace Network Route
```bash
traceroute google.com
```
Traces the route packets take to a destination.

### 4. Check Open Ports
```bash
netstat -tulnp
```
Displays active connections and listening ports.

### 5. Display Active Network Connections
```bash
ss -tulnp
```
Shows active TCP and UDP connections.

### 6. Display Routing Table
```bash
ip route show
```
Shows the current routing table.

### 7. Test DNS Resolution
```bash
nslookup google.com
```
or  
```bash
dig google.com
```
Resolves a domain name to an IP address.

### 8. Restart Network Services
```bash
systemctl restart NetworkManager
```
or  
```bash
/etc/init.d/networking restart
```
Restarts the network service.

### 9. Monitor Network Traffic
```bash
tcpdump -i eth0
```
Captures and displays live network traffic.

### 10. Check Network Interface Status
```bash
nmcli device status
```
or  
```bash
ifconfig
```
Displays network interface details.

---


