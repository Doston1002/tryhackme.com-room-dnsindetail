# tryhackme.com-room-dnsindetail

TryHackMe | DNS in Detail | Writeup

--------------------------Task 1 ----------------------------------------

What is DNS?
Answer: Domain Name System

--------------------------Task 2 ----------------------------------------

Domain Hierarchy

What is the maximum length of a subdomain?
Answer:63

Which of the following characters cannot be used in a subdomain ( 3 b _ - )?
Answer:_

What is the maximum length of a domain name?
Answer:253

What type of TLD is .co.uk?
Answer:ccTLD

--------------------------Task 3 ----------------------------------------

Record Types

What type of record would be used to advise where to send email?
Answer:MX

What type of record handles IPv6 addresses?
Answer:	AAAA

--------------------------Task 4 ----------------------------------------

Making A Request

What field specifies how long a DNS record should be cached for?
Answer:TTL

What type of DNS Server is usually provided by your ISP?
Answer:Recursive

What type of server holds all the records for a domain?
Answer:authoritative

--------------------------Task 5 ----------------------------------------

Practical

What is the CNAME of shop.website.thm?

user@thm:~$ nslookup --type=CNAME shop.website.thm
Server: 127.0.0.53
Address: 127.0.0.53#53

Non-authoritative answer:
shop.website.thm canonical name = shops.myshopify.com

Answer:shops.myshopify.com

What is the value of the TXT record of website.thm?

user@thm:~$ nslookup --type=TXT website.thm
Server: 127.0.0.53
Address: 127.0.0.53#53

Non-authoritative answer:
website.thm text = "THM{7012BBA60997F35A9516C2E16D2944FF}"

Answer:THM{7012BBA60997F35A9516C2E16D2944FF}

What is the numerical priority value for the MX record?

user@thm:~$ nslookup --type=MX website.thm
Server: 127.0.0.53
Address: 127.0.0.53#53

Non-authoritative answer:
website.thm mail exchanger = 30 alt4.aspmx.l.google.com

Answer:30


What is the IP address for the A record of www.website.thm?

user@thm:~$ nslookup --type=A www.website.thm
Server: 127.0.0.53
Address: 127.0.0.53#53

Non-authoritative answer:
Name: www.website.thm
Address: 10.10.10.10

Answer:10.10.10.10
