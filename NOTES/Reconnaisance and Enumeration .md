# Recon 

## What is Recon?
- It is the first phase of any hacking process.
- It involves gathering information about a target to identify vulnerabilities.
- Can be ,
  1. Passive (No direct interaction with the target).
  2. Active ( Direct interaction with the target).

## Types of Recon
1. Passive Recon
   - Eg: DNS queries, social media analysis, google dorking.
   - DNS query: A request sent by the dns client to the dns server to resolve a domain name into its corresponding IP address.
   - google dorking: process of using advance search operations to uncover hidden or sensitive information.
   - Tools:
     - google dorks
       - Advanced Search operation for sensitive information.
     - Whois
       - Domain registration and ownership information.
     - Shodan
       - Search Engine for IoT devices and Open ports.
2. Active Recon
   - Eg: Network scanning, ping sweeps, banner grabbing.
   - ping sweeps : network scanning technique used to identify which IP address corresponds to live hosts on the network.
   - banner grabbing:
   - Tools:
     - nmap
       - Network mapping, port scanning, service detection.
     - netcat
       - reading and writing data across networks, banner grabbing.
     - Nikto
       - A web browser scanner that checks for the outdated versions, vulnerable scripts, and other security issues on the webserver.
      
#### BEST PRACTICES
- Always start with passive methods for detection.
- Use anonymizing techniques(VPN, TOR) during active recon.
- Document all findings systematically for further analysis.

# Enumeration

## what is enumeration?
- gathering  detailed information about targets network and system after initial scanning.
- It helps identify things like username, shared files, software details that might be vulnerable.
- Enumeration is key in cyberseccurity to find weak spots that could be exploited.

### TYPES OF INFO GATHERED USING ENUMERATION
1. Network source
2. users and groups
3. The various machine names
4. Applications
5. DNS details

### PROCESS OF ENUMERATION
<img width="1138" height="854" alt="image" src="https://github.com/user-attachments/assets/ee8ae3fc-6f4f-41de-9501-1f75cb28c013" />

#### SMTP ENUMERATION
- SMTP(Simple Mail Transfer Protocol) enumeration is a technique used in penetration testing to gather information about a mail server, it's users, and possible vulnerabilities.
  - Purpose:
    - Identifies valid email addresses and user accounts.
    - Check for misconfigurations and vulnerabilities in the mail server.
     
#### SMTP-USER-ENUM
- SMTP-user-enum is a command-line-tool used to enumerate valid usernames on an smtp server
- by sending specific SMTP commands like
  - VRFY (asks the server to verify if a username exists)
  - EXPN  (expands a mailing list to show its members.
  - RCPT TO (checks if the server accespts mail for a given address.
- It helps identify existing email addresses for potential use in attacks like phishing or brute force.

- Installation:
  - git clone https://github.com/pentestmonkey/smtp-user-enum
 
### SNMP(Simple network management protocol)
- Is an internet standard protocol used to monitor and manage networks devices connected over an IP.
- It is used for communication between routers, firewalls, loadbalancers, servers, CCTV cameras and wireless devices.

### SNMP ENUMERATION
- Process of gathering information about devices on the  network using simple network management protocol(SNMP).

- Purpose:
  - To extract information about network devices such as:
    - System details(name, uptime, services)
    - Installed software and hardware configurations.
    - Active ports and processes.
   
#### SNMPWALK
- snmpwalk is a command-line tool used for querying and retrieving data from SNMP-enabled devices.
-  It works by performing a sequence of SNMP GETNEXT requests,
-   walking through a network device's Management Information Base (MIB) to gather detailed information.

- Installation:
  - sudo apt install snmp
 

### FTP (File Transfer Protocol)
-  is a standard network protocol used to transfer files between a client and a server over a TCP/IP network, such as the internet.

### FTP ENUMERATION
- Process of discovering valid FTP usernames and their associated permissions on a target system.

- Purpose:
  - Identify valid accounts.
  - Access the security posture of the FTP server.
    
 #### FTP ANONYMOUS LOGIN
 - Anonymous FTP allows users to access files without requiring a specific username or password.
 - using "anonymous" as the username and typycally an email address as a password.

######## Risks

- Unauthorized access:: Sensitive files may be exposed
- Data Theft: Potential for unauthorized downloading of data.
- Data Tampering: Users could potentially upload malicious files.

  ### SMB(Server Message block)
  - is a network file sharing protocol that enables users and applications to access files, printers, and other resources on the network.
  - 
  

                         
                         

