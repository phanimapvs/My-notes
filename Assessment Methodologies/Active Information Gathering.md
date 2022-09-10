## `Information Gathering` :monocle_face:  

***Active Information Gathering:***
  
  Actively Interacting with the target to gather the information about it by pinging and scanning [Requires Authorization to perform Active Recon]. 
  
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
