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

![1](https://github.com/sathyaa22/Enumeration/assets/140483368/b9256bc0-3b2c-485b-a8b8-4260317e34a5)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![2](https://github.com/sathyaa22/Enumeration/assets/140483368/4f5dd4c4-d9bb-416b-97eb-5c7a084b7e69)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![3](https://github.com/sathyaa22/Enumeration/assets/140483368/f81bc6f4-f823-46c5-89c2-40665583ed87)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![4](https://github.com/sathyaa22/Enumeration/assets/140483368/d62ae509-ee81-41f3-b9ce-db925cde6a1f)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![5](https://github.com/sathyaa22/Enumeration/assets/140483368/dc52c2b8-8552-49cc-bc9d-b81eebfb4073)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![6](https://github.com/sathyaa22/Enumeration/assets/140483368/2e5e09e3-13c0-43f7-83e9-2734411e34ec)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![7](https://github.com/sathyaa22/Enumeration/assets/140483368/c0294f1d-7c15-4b7c-9b7d-0be5b9c96aca)

 
#DNS Enumeration

##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:


![8](https://github.com/sathyaa22/Enumeration/assets/140483368/a2bac13e-b9cf-4f90-ad95-780d095be727)


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

![9](https://github.com/sathyaa22/Enumeration/assets/140483368/f362cdb4-152f-4cb5-b39d-b735aef7e859)

![10](https://github.com/sathyaa22/Enumeration/assets/140483368/dfaaa8aa-6bca-42f6-9780-30a446bc58ec)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![11](https://github.com/sathyaa22/Enumeration/assets/140483368/a848af2a-61fb-43ff-bf1d-889324bac668)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![12](https://github.com/sathyaa22/Enumeration/assets/140483368/1b56d778-d9c5-4185-ba75-058ac40d4718)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
##Output
  
![13](https://github.com/sathyaa22/Enumeration/assets/140483368/4217fabd-f4ed-4160-b3cb-581dc5b17df3)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:

![output](https://github.com/sathyaa22/Enumeration/assets/140483368/8606f09d-b4cd-4d35-b635-c0d630dbabf6)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

