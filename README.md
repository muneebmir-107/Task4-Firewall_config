#  Cyber Security Internship – Task 4: Firewall Configuration (Windows)

## Task Objective
Configure and test basic firewall rules using **Windows Defender Firewall** to allow or block traffic.


## System Used
- **Operating System**: Windows 10  
- **Firewall Tool**: Windows Defender Firewall (Advanced Settings)  
- **Testing Tool**: Nmap (for port scanning)


## Steps Performed

### 1. Accessed Firewall Settings
- Opened **Windows Defender Firewall with Advanced Security**.
- Navigated to **Inbound Rules** to view existing rules.

### 2. Blocked Port 23 (Telnet)
- Created a **new inbound rule**:
  - Rule type: Port → TCP → Port: `23`
  - Action: **Block the connection**
  - Profile: Domain, Private, Public
  - Name: `Block Telnet`


### 3. Tested Using Nmap
- Ran the following command to test port status:
  nmap -p 23 localhost

### 4. Result:
Port 23: Reported as closed
