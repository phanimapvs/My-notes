## `Information Gathering` :monocle_face:  

***Passive Information Gathering:*** 
  
  Gathering the information about the target without directly interacting with the target. It involves gathering the information from various publicly available sources such as Google, Linkedin, Facebook etc

 - ***Find IP addresses & DNS information***
 
    - ***DNSRECON TOOL:***

       `dnsrecon` is a Kali linux tool that will gives us the data about the NS[Name server], MX[Mail server], A[Ipv4], AAAA[Ipv6] etc
       
       Usage: `dnsrecon -d [target domain]`

       ![image](https://user-images.githubusercontent.com/42320878/189398598-5cc92c72-9983-4f74-8557-b8453502089f.png)
       
    - ***DNSDUMPSTER WEBSITE:*** 
    
       Same applications as dnsrecon but more affective
       
       ![image](https://user-images.githubusercontent.com/42320878/189400495-e4765a31-3cd6-47a6-93c4-35180a571bc9.png)
       
       ![image](https://user-images.githubusercontent.com/42320878/189400993-59b27cf4-3930-4213-aca9-86e99397a01d.png)


 
 
    - ***Using host tool to get IP:***
 
       ![image](https://user-images.githubusercontent.com/42320878/189367135-f8909e58-7f16-4ca0-a2d4-e017554e3f62.png)


    - ***Domain names and Domain Ownership information***
 
    -  Whois Lookup [Can be done from terminal or from a webapp]
      
      ![image](https://user-images.githubusercontent.com/42320878/189373435-74993ee1-6339-4dcd-8b8c-0e3243cbfad5.png)
      
      ![image](https://user-images.githubusercontent.com/42320878/189374281-abfcfdcf-ff2c-4aa2-a2a9-bc4d17e39833.png)


 - ***Identifying the Sub-domains***
 
    - [Virustotal](https://www.virustotal.com/) website can be used to find the subdomains. 
    - Sublist3r
    - Ffuf
    - dirb
    - Dirbuster
    - Google Dorks & GOOGLE HACKING DATABASE
      - site:*.google.com 
      - site:*.google.com inurl:admin
      - site:*.google.com intitle:admin
    - waybackmachine
    
 - ***Identifying Emails, Phone numbers and Social media profiles***
    
    - theHarvester [a Kali linux tool]
    - hunter.io [A web application for Email gathering ]

- ***Web technologis that are being used by the target***

     - ***Whatweb*** [A tool in Kali linux] | `Usage: whatweb [Target URL]`
     
     - ***Builtwith*** (Add-on)
     
     - ***Wappalyzer*** (Add-on)
     
     - ***Webhttrack*** [A Linux tool] : Can be used to Download the Entire website. Useful to analyze the source code of the target website.
     
     ![image](https://user-images.githubusercontent.com/42320878/189370732-827cda10-e725-46d8-9237-56a4cd3ad11c.png)

 ## Others:
 
   ***Netcraft***
   
   Netcraft can be used to identify the WhoIs Data of the Website along with the data of SSL and TLS certificates.
   It can gather IP related information, web trackers, site technologies etc.. [ ALL INFO AT ONE PLACE i.e, NetCraft ]
   
   ![image](https://user-images.githubusercontent.com/42320878/189394856-16ae863b-9f4d-4975-bb91-4cfca7d85f14.png)
   
   If the website is vulnerable to any of the exploits we can check that from the below section
   
   ![image](https://user-images.githubusercontent.com/42320878/189396728-25035a70-1e4e-484e-a3a4-8954d4d8158d.png)
   
   Technologies that the website is using
   
   ![image](https://user-images.githubusercontent.com/42320878/189397270-0945ab33-316e-4616-bd14-ed3f650ad362.png)

   `wafw00f`is a kali linux tool that Identifies if the website is WAF protected or not 
   
   ![image](https://user-images.githubusercontent.com/42320878/189408656-66a8056d-6aff-4878-9ddc-3fefc1675204.png)
   
   ![image](https://user-images.githubusercontent.com/42320878/189408959-3e56879b-1557-42ec-8642-936dc673a8c6.png)



 
   ***Robots.txt***
   
   ![image](https://user-images.githubusercontent.com/42320878/189365622-2969f98e-05ff-471e-bc21-7c4d13c64b1e.png)
   
   ***sitemap.xml***
   
   ![image](https://user-images.githubusercontent.com/42320878/189368017-a03dc1fc-b78f-49e7-b796-71c04fcbb73e.png)

   ***haveibeenpwned.com***
   
   Its used to check the data we have with the data that was breached
   
   ![image](https://user-images.githubusercontent.com/42320878/189415448-dd262dd9-0329-4033-a1b8-7efe7264c3d4.png)

