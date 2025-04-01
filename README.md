Project Goal

I conducted a DNS record investigation to analyze publicly available data on the tryhackme.com domain. The project's goal is to study the domain's infrastructure, identify subdomains, mail servers, and other key information that can be used in penetration testing or cyber reconnaissance.

Process Description

To achieve the goal, I used several tools:

nslookup – to retrieve information about DNS records.

dig – to perform queries to DNS servers and analyze MX records.

DNSDumpster – an online service for DNS reconnaissance and subdomain enumeration.

Research Results

Identified Subdomains:

blog.tryhackme.com

insights-proxy-worker.tryhackme.com

remote.tryhackme.com

www.tryhackme.com

MX Records (Mail Servers):

aspmx.l.google.com

alt1.aspmx.l.google.com

alt2.aspmx.l.google.com

alt3.aspmx.l.google.com

alt4.aspmx.l.google.com

NS Records (Name Servers):

uma.ns.cloudflare.com

kip.ns.cloudflare.com

TXT Records (Verification and SPF Policy):

google-site-verification=umR4x8HuzWMF5g3656JY1b-61NuryD0-GqGnYN13ONo

v=spf1 include:_spf.google.com include:email.chargebee.com include:7168674.spf05.hubspotemail.net ~all

Conclusion

The research showed that the tryhackme.com domain is protected by Cloudflare, uses Google mail servers, and has several subdomains that may contain potentially valuable information. These findings can be useful for penetration testing or further OSINT analysis.

Future steps could include:

Using Sublist3r or amass to search for hidden subdomains.

Checking open ports on discovered IPs with Nmap.

Investigating web applications on subdomains using WhatWeb or Gobuster.

This project provided me with hands-on experience using DNS reconnaissance tools and expanded my knowledge in cybersecurity.
