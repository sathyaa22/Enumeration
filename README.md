# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

![1](https://github.com/gowriganeshns/Enumeration/assets/140483368/cf48074d-d84b-4e3c-94f9-c3e1da1d9fd5)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![2](https://github.com/gowriganeshns/Enumeration/assets/140483368/f0e88ca6-6e81-4952-b34d-7936836db403)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![3](https://github.com/gowriganeshns/Enumeration/assets/140483368/f325ddb4-fafc-4b4d-8cde-1d4b774258cd)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![4](https://github.com/gowriganeshns/Enumeration/assets/140483368/26b4b478-55cd-4ef1-a047-61bd937cabeb)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![5](https://github.com/gowriganeshns/Enumeration/assets/140483368/e6644b75-8bec-4e56-877e-6f735532b3cf)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![6](https://github.com/gowriganeshns/Enumeration/assets/140483368/d8bea31f-f712-4dc2-8783-8046575c150f)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![7](https://github.com/gowriganeshns/Enumeration/assets/140483368/e24dab98-4d2e-46c3-a2ca-7940ba6abf07)

#DNS Enumeration
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![8](https://github.com/gowriganeshns/Enumeration/assets/140483368/76f78862-2196-432b-8759-ce50be63dc47)


##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

![9](https://github.com/gowriganeshns/Enumeration/assets/140483368/e61db38a-5788-4127-a396-8c5f8f4a8218)

![10](https://github.com/gowriganeshns/Enumeration/assets/140483368/5c062dfa-616a-45b3-b118-084a789809f0)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![11](https://github.com/gowriganeshns/Enumeration/assets/140483368/5c179f20-e452-47e5-b3ea-b55ca246a6a1)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![12](https://github.com/gowriganeshns/Enumeration/assets/140483368/0defd73e-3db0-4f41-953a-ada07a4f7d50)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
##Output
  
![13](https://github.com/gowriganeshns/Enumeration/assets/140483368/f971269a-5932-4414-ac42-585d183600c4)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![output](https://github.com/gowriganeshns/Enumeration/assets/140483368/c17898b2-1a75-4357-9a9d-efdc7ba77968)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

