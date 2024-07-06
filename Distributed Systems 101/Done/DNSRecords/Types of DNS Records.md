## Common Types 
A - An address think 192.168.1.1.
	- nullcloud.io - a -> 72.10.2.87
PTR - or pointer - opposite of above, lets you map an IP to domain name (not common I don't think)
AAAA - Same as A, but IPV6.
CNAME - Canonical name - A dns record that points to another DNS Record. (think sub domains ect)
	- dev.nullcloud.io -> nullcloud.io
NS - The definitive name server, usually you have 2, a primary and secondary
MX - Mail Exchange - this is where e-mails to this domain should go
TXT - Text - you can store text in this. some use it to authenticate authority of a domain.
 - here is a special string just for you "asdfjkl"
 - TXT -> "asdfjkl"

Uncomon:
SOA - common, but is more for the DNS server.
SPF - something to do with protecting e-mail from spammers. People ether don't use it or it does not work... just saying.
APL - Not Apples 

references: 
https://www.cloudflare.com/learning/dns/dns-records/
https://en.wikipedia.org/wiki/List_of_DNS_record_types