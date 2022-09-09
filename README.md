# `Pentetration testing Notes` :smiling_face_with_three_hearts:

The Phases of Penetration testing
  - Information gathering / Reconnaissance
  - Scanning
  - Enumeration
  - Exploitation
  - Privilege Escalation & Post Exploitation Tactics
  - Clearing Tracks

![image](https://user-images.githubusercontent.com/42320878/189353053-459bc450-07f5-4ac8-877a-20597c20d5ae.png)

## `Information Gathering` :monocle_face:  

***Passive Information Gathering:*** 
  
  Gathering the information about the target without directly interacting with the target. It involves gathering the information from various publicly available sources such as Google, Linkedin, Facebook etc

 - ***Find IP addresses & DNS information***
 
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
    
 - Identifying Emails, Phone numbers and Social media profiles

- ***Web technologis that are being used by the target***

     - ***Whatweb*** [A tool in Kali linux] | `Usage: whatweb [Target URL]`
     
     - ***Builtwith*** (Add-on)
     
     - ***Wappalyzer*** (Add-on)
     
     - ***Webhttrack*** [A Linux tool] : Can be used to Download the Entire website. Useful to analyze the source code of the target website.
     
     ![image](https://user-images.githubusercontent.com/42320878/189370732-827cda10-e725-46d8-9237-56a4cd3ad11c.png)

 ## Others:
 
   ***Robots.txt***
   
   ![image](https://user-images.githubusercontent.com/42320878/189365622-2969f98e-05ff-471e-bc21-7c4d13c64b1e.png)
   
   ***sitemap.xml***
   
   ![image](https://user-images.githubusercontent.com/42320878/189368017-a03dc1fc-b78f-49e7-b796-71c04fcbb73e.png)




***Active Information Gathering:***
  
  Actively Interacting with the target to gather the information about it by pinging and scanning [Requires Authorization to perform Active Recon]. 
  
  - Discover the open ports and services of the target system
  - Learning about internal infrastructure of a target network/Organization
  - Enumerating the Information from target systems 
    

