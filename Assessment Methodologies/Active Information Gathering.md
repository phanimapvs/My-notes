## `Information Gathering` :monocle_face:  

***Active Information Gathering:***
  
  Actively Interacting with the target to gather the information about it by pinging and scanning [Requires Authorization to perform Active Recon]. 
  
  ![image](https://user-images.githubusercontent.com/42320878/189477859-d88a32ef-f818-4371-b507-7cb1fa783060.png)     
  
  - Discover the open ports and services of the target system
  - Learning about internal infrastructure of a target network/Organization
  - Enumerating the Information from target systems 

***DNS Interrogation***

DNS interrogation is a process of enumerating DNS records of specific domain. it provides information such as IP Address of the domain, Subdomains, mail servers etc...

   ***DNS Zone transfer***
    
   DNS zone transfer is a feature that is utilized by server admins to transfer the zone files from one server to another. A zone file consists the DNS records of the domain. If this feature is misconfigured then attackers can take the advantage of this feature to get the DNS records that they are not supposed to get...


***DNS Records:***

  - A : Resolves a hostname to the IPv4 address
  - AAAA : Resolves a domain or a hostname to IPv6 address
  - NS : Reference to the domains nameserver
  - MX : Resolves a domain to a mail server
  - CNAME : Used for domain aliases
  - TXT : Text record
  - HINFO : Host information
  - SOA : Domain authority
  - SRV : Service records
  - PTR : Resolves an IP address to a hostname 

***Tools:***

`dnsenum`

![image](https://user-images.githubusercontent.com/42320878/189474489-395c8f44-1017-4f95-87e5-bd904fb26fd0.png)

![image](https://user-images.githubusercontent.com/42320878/189474945-841627a9-6695-4468-8aed-51de0872799b.png)


`dig`

![image](https://user-images.githubusercontent.com/42320878/189475252-be7c566e-1c08-4bb8-970d-5f4dfe3db9ae.png)


`fierce`

![image](https://user-images.githubusercontent.com/42320878/189475331-e91fa0cc-e309-4caf-91e5-272e01cd1222.png)



## ***`Scanning the Network`*** :mag:

Command: `nmap -sn [IP Address]` | It tells the nmap to scan network with no portscan[sn] 

![image](https://user-images.githubusercontent.com/42320878/189475570-e5c594a2-df87-4283-b9e0-2599aaa57897.png)

***Default Network Scan with Nmap***

When we perform the default Nmap scan on a **`Windows machine`** as the Windows machine blocks the ICMP packets.. it will show **`the host is down`** So, we can directly perform the port scan without seeing if the host is up or not if the target machine is a Windows machine. default scan will scan the top 1000 ports among 65535 ports.

![image](https://user-images.githubusercontent.com/42320878/189475920-3a783a02-4c74-4bb4-b8ad-2b1470912393.png)

***Other Common Scanning Syntax:***

**Syntax**    |    **Description**
----    |    -----
nmap -p- 10.10.1.2 | Scans all the 65535 ports as the ports in syntax is mentioned as `-p-`
nmap -F 10.10.1.2 | It is known as fast scan and it Scans the top 100 ports
nmap -p 80,443,22 10.10.1.2 | Scanning the Custom ports  
nmap -sU 10.10.1.2 | UDP Scan
nmap -p 80,443,22 -sV 10.10.1.2 | Service version detection on custom ports
nmap -p 80,443,22 -sV -O 10.10.1.2 | Scan for Operating System detection along with service versions
nmap -p 80,443,22 -sV -O -sC 10.10.1.2 | Uses the nmap Scripts along with the above scan
nmap -A -p- 10.10.1.2 | Scans the service numbers, Operating systems and uses scripts on all ports
nmap -A -T4 -p- 10.10.1.2 -v | Scans all ports and services within the given time frame `T4` and results the verbose
nmap -A -p- 10.10.1.2 -oN Output.txt | **Normal Format:** Outputs the scan info to the Output.txt file
nmap -A -p- 10.10.1.2 -oX Test.xml | **Xml Format:** Outputs the scan info to the Test.xml file. Xml files can be later imported into Metasploit framework


