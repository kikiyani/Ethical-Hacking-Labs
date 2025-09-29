###### ########## Finding DNS and Subdomain information ########### ######


DomainTools WHOIS lookup service — a web interface that returns registration and related historical information about a domain or IP (who registered it, registrar, name servers, registration/expiry dates, and related metadata). i Preffered not entering my results to this lab here as it contains sensitive informtaion. 
1. WHOIS can show registrant names/emails. An attacker can craft phishing/spearphishing targeting those addresses if they’re exposed.
2. Reverse-WHOIS reveals other domains registered to the same contact (extra targets the organization forgot about).
3. Hosting/IP history shows past hosts or IPs where backups or old content might still be reachable (useful to find forgotten sites).
4. Name servers and registrar details help map vendor relationships and weaker third-party sites (supply-chain entry points).
<img width="1307" height="488" alt="image" src="https://github.com/user-attachments/assets/30af595f-c5d4-4f92-92d9-9d725d1423f8" />
Information i came across:
Registrar info → If the registrar has weak security or no MFA, attackers might attempt registrar account takeover.
Registrant info → If WHOIS privacy wasn’t enabled, personal names/emails could be used for phishing/social engineering. Here it’s redacted, so safer.
Creation/expiry dates → Attackers may monitor domains close to expiry to try domain hijacking if the owner forgets to renew.
Name servers → Show that DNS is on Google Cloud → attacker knows the hosting/DNS provider. They might look for misconfigurations (like dangling subdomains).
Domain status locks → If these weren’t set, hijacking would be easier. Their presence makes it harder.
History (not shown here, but available in services like DomainTools) → Past owners, old registrant emails, or infrastructure changes can help attackers pivot.

##############################################################################################################################################################

ViewDNS.info is a one-stop, web-based OSINT toolbox for DNS / domain / IP investigation. It provides many free lookups (and paid APIs) you can use to enumerate DNS records, WHOIS data, reverse-IP/NS, subdomains, IP history, traceroute, HTTP headers, blacklist checks, and more — useful for both defenders and attackers during reconnaissance
<img width="1271" height="532" alt="image" src="https://github.com/user-attachments/assets/188f95b9-8a1e-45c3-9b5c-e6689f4f7853" />
IP HISTORY: 
Each line shows an IP address that the target org has pointed to at some time, the ISP/owner of that IP, the geolocation, and the date the domain was last seen there. That gives a timeline of where the site has been hosted and who hosted it.
<img width="1203" height="307" alt="image" src="https://github.com/user-attachments/assets/c2d11028-4ed5-4977-88d8-811cb7649225" />
SUBDOMAIN DETAILS: For many subdomains you see an IP address and a recent resolution date — those are live and currently resolve.
<img width="1218" height="326" alt="image" src="https://github.com/user-attachments/assets/2f5c9cc6-2fc4-41fd-9d30-efab796ead0a" />



############################################################################################################################################################
DNSDumpster is a free web-based OSINT tool for DNS/domain reconnaissance. You paste a domain into the site and it returns a compact “attack-surface” view: DNS records, host→IP mappings, reverse-IP insights, historical/related hosts, ASN/ISP info and a visual network map. It’s used by both red teams and blue teams to map public infrastructure.
<img width="1333" height="477" alt="image" src="https://github.com/user-attachments/assets/dd516332-c604-494d-85e4-fa22c6ef2d89" />
<img width="1040" height="400" alt="image" src="https://github.com/user-attachments/assets/8282ce93-4b4f-4d79-90fe-5f24fb0366a3" />





