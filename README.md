# CyBot
Open Source Threat Intelligence Chat Bot

Threat intelligence chat bots are useful friends. They perform research for you and can even be note takers or central aggregators of information. However, it seems like most organizations want to design their own bot in isolation and keep it internal. To counter this trend, our goal was to create a repeatable process using a completely free and open source framework, an inexpensive Raspberry Pi (or even virtual machine), and host a community-driven plugin framework to open up the world of threat intel chat bots to everyone from the home user to the largest security operations center.

We are excited to share with the world a chat bot that we affectionately call CyBot. We will show you what CyBot can do for you and graciously accept feedback on future improvements. Best of all, if you know even a little bit of Python, you can help write plugins and share them with the community. If you want to build your own CyBot, the instructions in this project will let you do so with about an hour of invested time and anywhere from $0-$35 in expenses--quite a good return on your investment.


# CyBot Plugins

 **== File commands ==**

 !vt <hash> - VirusTotal Query (ex: 57f222d8fbe0e290b4bf8eaa994ac641)  
 !hashid <hash> - Identify a hash type (e.g. MD5, SHA1) (Props:  c0re)  

 **== Network commands ==**

 !vt <URL> - VirusTotal Query
 !safebrowsing <URL> - Google Safebrowsing lookup (ex:  ihaveaproblem[.]info) (Props: Google)  
 !whois <domain> - WHOIS Query (ex: cylance[.]com) (Props:  hackertarget[.]com)  
 !nslookup <FQDN|IP> - DNS forward/reverse Query (ex: www[.]cylance[.]com)  
 !geoip <FQDN|IP> - Perform GeoIP lookup of host (ex: www[.]cylance[.]com) (Props: freegeoip[.]net)  
 !unshorten <shortened URL> - Unshortens URLs (ex: goo[.]gl/IGL1lE)  
 !linkextractor <FQDN|IP> - Extracts links from a site and safely displays them (ex: hxxps://www[.]google[.]com)  
 !urldecode <url> - Decodes encoded URLs (ex: /%75%72%6C?%73%61=%74)  

 **== Misc ==**

 !secnews - (Use as Private Message Only) Latest security news (Props: Google News - CyberSecurty)  
 !vulnnews - (Use as Private Message Only) Latest vulnerability news (Props:  Google News - CVE Vulnerability)  
 !time <timezone> - Query time in specified timezone (ex: utc)  
 !weather <zipcode> - Query the weather in a specified zip code (ex: 21144)  
 !unixtime <epoch> - Convert Unix time (seconds since Jan 1, 1970) to human readable (ex: 1347517370)  
 !calc <arithmetic input> - Performs basic arithmetic (Valid input: [0-9]+-/)  (ex: 22*3)  
 !bitcoin - Polls the latest Bitcoin Price Index (Props: CoinDesk)  
 !codename - Generates a 2 word project codename (Props: Mark Biek)  


# Setup steps
1)  Download and install errbot:  http://errbot.io/en/latest/user_guide/setup.html#prerequisites

2)  Configure errbot to work with your chat platform:  http://errbot.io/en/latest/user_guide/setup.html#id1

3)  Download our plugins from this github repo and copy them into the errbot plugins directory

4)  Add VirusTotal and Google Safebrowsing API keys to python scripts

5)  Start errbot


# Props
Errbot developers for the fantastic tool and customer service  
VirusTotal  
geoip - freegeoip.net  
Google Safebrowsing - https://developers.google.com/safe-browsing/ and Jun C. Valdez
Hashid - C0re  
Unshorten - unshorten.me  
Codename - https://mark.biek.org/code-name/
Black Hat Arsenal team for the amazing support and tool release venue

People:  Bill Hau, Corey White, Dennis Hanzlik, Ian Ahl, Dave Pany, Dan Dumond, Kyle Champlin, Kierian Evans, Andrew Callow, Mark Stevens
