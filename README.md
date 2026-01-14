# Security-Testing-Playbook
  Security foundation notes

### Q1. What is IANA (Internet Assigned Numbers Authority)?
        Responsible for Global internet identifiers such as IP address blocks [192.168.1.0/24(ipv4),
        8.8.8.0(organization ip-ISP style)], Port numbers (http/80,https/443, ftp/21, ssh/22), protocol parameters (TCP/6, UDP/17, ICMP/1).
            	
              IANA [(controlled by ICAAN (multi stake-holder model)] -> Regional Internet Registries -> ISPs -> us
              
              ###  IANA matters because:
                
                1.	Port to service assumption
                2.	Protocol consistency
                3.	DNS hierarchy[translate human-friendly domain names into IP addresses.{Root level(.) -> TLD(.com,.org,.in) -> Authoratative name server(A/AAAA, CNAME, MX record)-> Recursive resolver(ISP, cloudflare)}]

               ### DNS hierarchy matters:

                1.Subdomain enumeration abuses hierarchy
                2.Zone transfers leak authoritative data
                3.Cache poisoning targets resolvers
                4.Misconfigured DNS exposes internal assets
<p align="center">
  <img
    src="https://github.com/script-kiddie-005/script-kiddie-005/blob/main/CS_img.jpeg?raw=true" width=1000 height=200>
</p>
                
        Well-known ports (0–1023)
        Registered ports (1024–49151)
    
