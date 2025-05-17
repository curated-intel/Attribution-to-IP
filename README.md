# Attribution to IP
- A collection of methods to learn who the owner of an IP address is.

## OSINT & Freemium Services
> [!NOTE]
> These are free methods, but paid accounts may be available for some of these services for more information, authenticated APIs, and higher rate limits.

| Method | Description | Source(s) |
| --- | --- | --- |
| Passive DNS (pDNS) | Shows historical DNS resolutions for an IP and allows you to identify domains that have pointed to the IP. | [ViewDNS.info](https://viewdns.info) / [VirusTotal](https://www.virustotal.com)  / [OTX AlienVault](https://otx.alienvault.com/) / [Mnemonic](https://passivedns.mnemonic.no/) / [DNSlytics](https://search.dnslytics.com/) |
| Domain DNS Records | Includes A, PTR, MX, TXT, and CNAME records. PTR records can reveal the hostname; TXT and MX can give clues about the domain’s owner or provider. | [ViewDNS.info](https://viewdns.info) / [CentralOps](https://centralops.net/co/) / [DNSlytics](https://search.dnslytics.com/) / [DNSDumpster](https://dnsdumpster.com/) |
| IP WHOIS | Queries registrar and network block registration info. Can directly identify the entity or ISP that registered the IP range. | [ViewDNS.info](https://viewdns.info) / [DomainTools](https://whois.domaintools.com/) / [CentralOps](https://centralops.net/co/) / [Who.is](https://who.is/) |
| Open Ports & Running Services | Scanning the IP for accessible ports and services. Banner grabbing can reveal software, versions, and sometimes organization names. | [Shodan](https://www.shodan.io/) / [FOFA](https://en.fofa.info/) / [Censys](https://search.censys.io/) / [Onyphe](https://search.onyphe.io/) |
| SSL Certificates | Examine SSL certs served on open HTTPS ports. Certs often contain domains, email addresses, or organization names. | [Certificate Search](https://crt.sh) / [Censys](https://search.censys.io/) |
| Autonomous System Names (ASNs) | ASNs describe ownership of blocks of IP addresses. Helps identify the ISP, hosting provider, or large organization behind a network. | [IPinfo](https://ipinfo.io/) / [InfoByIP](https://www.infobyip.com/) / [IPQS](https://www.ipqualityscore.com/) / [Shodan](https://www.shodan.io/) / [FOFA](https://en.fofa.info/) / [Censys](https://search.censys.io/) / [Onyphe](https://search.onyphe.io/) |
| IP Geolocation | Maps IP to approximate physical location. Helps determine country or city, which may assist in narrowing the scope of who the owner is. | [MaxMind](https://www.maxmind.com/en/geoip-demo) / [IPinfo](https://ipinfo.io/) / [InfoByIP](https://www.infobyip.com/) / [IPQS](https://www.ipqualityscore.com/) / [Shodan](https://www.shodan.io/) / [FOFA](https://en.fofa.info/) / [Censys](https://search.censys.io/) / [Onyphe](https://search.onyphe.io/) |
| Border Gateway Protocol (BGP) | BGP announcements tell you who is routing the IP block and confirms the autonomous system or network managing the address. | [BGP Hurricane Electric](https://bgp.he.net/) / [BGP Tools](https://bgp.tools/) |
| Content Archives | Archived content of websites hosted on the IP and may show earlier branding, contact info, or domains before a site changed. | [URLscan](https://urlscan.io/) / [Wayback Machine](https://web.archive.org/) |
| Manual Browsing | Visiting the IP directly in a browser can sometimes reveals landing pages, admin panels, or redirect behavior with company names or logos. | [Browserling](https://www.browserling.com/) |
| Google Dorking | Use advanced search operators to find references to the IP online that could be used to identify its owner. | [Google Dork Examples](https://github.com/BushidoUK/OSINT-SearchOperators/blob/main/GoogleDorks.csv) |
| Code Repositories | Search in code repositories for references to the IP as the developers sometimes hardcode IPs in their code and configuration files. | [GitHub](https://github.com/) / [BitBucket](https://bitbucket.org/) |
| Linked to Tor Nodes, VPNs, or Proxies | Checking in lists of Tor, VPNs, or Proxy nodes suggests the IP is not owned by a specific end-user but part of a privacy or anonymisation network. | [TOR Node List](https://dev.dan.me.uk/tornodes) / [IPQS](https://www.ipqualityscore.com/) / [Spur](https://spur.us/context/me) |

## Commercial
> [!WARNING]
> These are paid services only typically available for enterprises or public sector organisations and provide more information and authenticated APIs.

| Method | Description | Source(s) |
| --- | --- | --- |
| NetFlow |  | [Team Cymru Pure Signal](https://www.team-cymru.com/) |
| Breach Data |  | [SpyCloud](https://spycloud.com/)  |
