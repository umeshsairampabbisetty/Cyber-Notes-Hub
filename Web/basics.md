DNS -> Domain Name System
    gives a domain instead of just remembering an ip
    
*Domain Hierarchy* (total max 253)
1st -> Root Domain -ex: .
2nd -> top level domain -ex: .com .edu .org
        2 types of tlds are gtld(general) and cctld(country code)
3rd -> second level domain -ex: youtube google gmail (max 63)
4th -> Subdomain it sits on the left-hand side of the Second-Level Domain using a period to separate it (max 63)

-Records- (use nslookup)
A -> resolves ipv4 adresses
AAAA -> resolves ipv6 adresses
CNAME -> resolves to another domain name
MX -> Resolves to the address of the servers that handle the email
TXT -> Holds data that verifies ownership or proves your outgoing emails are 
        legitimate.

-DNS Request Resolution Steps-
1st-Client / Local Cache
    Computer checks its own local cache first.
      If not found, then next step.
2nd-Recursive DNS Server (Resolver)
    Provided by ISP or configured manually.
     Checks its own cache (e.g., for popular sites like Google, Facebook).
      If not cached, goes next step.
3rd-Root DNS Server
    Serves as the DNS backbone of the internet.
     Reads domain extension (e.g., .com) and redirects to the corresponding TLD (Top Level Domain) Server.
4th-TLD DNS Server
    Stores records for specific domain extensions (.com, .org, etc.).
     Points to the specific Authoritative DNS Server (Nameserver) for the requested domain (e.g., kip.ns.cloudflare.com).
5th-Authoritative DNS Server
    Holds the actual DNS records for the specific domain name.
    Sends the requested IP address back to the Recursive DNS Server.
Final-Caching & Relay back to Client
    Recursive DNS Server caches the result locally for a duration set by the TTL (Time To Live) value (in seconds).
     Relays the IP address back to the Client to establish the connection.

