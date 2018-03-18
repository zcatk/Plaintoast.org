---
layout: default
title: "DNS Black Hole"
categories: pfsense
---

# DNSBL

## Current Lists

### Pihole DNSBL
```pihole
https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts
https://mirror1.malwaredomains.com/files/justdomains
http://sysctl.org/cameleon/hosts
https://zeustracker.abuse.ch/blocklist.php?download=domainblocklist
https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt
https://hosts-file.net/ad_servers.txt
```
### Adult DNSBL
```adult
https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/porn/hosts
https://raw.githubusercontent.com/chadmayfield/pihole-blocklists/master/lists/pi_blocklist_porn_top1m.list
```
### Malicious DNSBL
```Malicious
https://raw.githubusercontent.com/ZeroDot1/CoinBlockerLists/master/hosts
https://v.firebog.net/hosts/Airelle-hrsk.txt
https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt
https://hosts-file.net/exp.txt
https://hosts-file.net/emd.txt
https://hosts-file.net/psh.txt
https://mirror.cedia.org.ec/malwaredomains/immortal_domains.txt
https://www.malwaredomainlist.com/hostslist/hosts.txt
https://bitbucket.org/ethanr/dns-blacklists/raw/8575c9f96e5b4a1308f2f12394abd86d0927a4a0/bad_lists/Mandiant_APT1_Report_Appendix_D.txt
https://v.firebog.net/hosts/Prigent-Malware.txt
https://v.firebog.net/hosts/Prigent-Phishing.txt
https://raw.githubusercontent.com/quidsup/notrack/master/malicious-sites.txt
https://ransomwaretracker.abuse.ch/downloads/RW_DOMBL.txt
https://v.firebog.net/hosts/Shalla-mal.txt
https://isc.sans.edu/feeds/suspiciousdomains_Low.txt
https://isc.sans.edu/feeds/suspiciousdomains_Medium.txt
https://isc.sans.edu/feeds/suspiciousdomains_High.txt
```
### Ads DNSBL
```ads
https://adaway.org/hosts.txt
https://raw.githubusercontent.com/StevenBlack/hosts/master/data/UncheckyAds/hosts
https://filters.adtidy.org/extension/chromium/filters/15.txt
https://v.firebog.net/hosts/AdguardDNS.txt
http://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt
```
### Suspicious DNSBL
```suspicious
https://hosts-file.net/grm.txt
https://reddestdream.github.io/Projects/MinimalHosts/etc/MinimalHostsBlocker/minimalhosts
https://raw.githubusercontent.com/StevenBlack/hosts/master/data/KADhosts/hosts
https://raw.githubusercontent.com/StevenBlack/hosts/master/data/add.Spam/hosts
https://v.firebog.net/hosts/static/w3kbl.txt
https://v.firebog.net/hosts/BillStearns.txt
https://www.dshield.org/feeds/suspiciousdomains_Low.txt
https://raw.githubusercontent.com/piwik/referrer-spam-blacklist/master/spammers.txt
https://hostsfile.org/Downloads/hosts.txt
https://raw.githubusercontent.com/Dawsey21/Lists/master/main-blacklist.txt
https://raw.githubusercontent.com/vokins/yhosts/master/hosts
```
### Tracking / Telemetry / Fake-news DNSBL
```ttfn
https://v.firebog.net/hosts/Airelle-trc.txt
https://v.firebog.net/hosts/Prigent-Ads.txt
https://raw.githubusercontent.com/quidsup/notrack/master/trackers.txt
https://raw.githubusercontent.com/StevenBlack/hosts/master/data/add.2o7Net/hosts
https://raw.githubusercontent.com/StevenBlack/hosts/master/data/tyzbit/hosts
https://gist.githubusercontent.com/CHEF-KOCH/080efada22b9659ef61241029122873b/raw/7f9bd984d3c46b3dba2de7606da579bc0ac6780c/Canvas%2520Font%2520Fingerprinting%2520pages%2520%255B2017%2520Edition%255D
https://gist.githubusercontent.com/CHEF-KOCH/5a7b1593d1880f906b12a3c87cee4500/raw/3ba028508feb2ef67a3d7ab75f428fd284223e8b/WebRTC%2520tracking%2520list%2520%255B2017%2520Edition%255D.txt
https://gist.githubusercontent.com/CHEF-KOCH/63fd2e506cb34a2378ad2620ab06d2e0/raw/fb9f16e3ac998d3f773ebdfee4aa3bfd10a5d763/Audio%2520fingerprint%2520pages%2520%255B2017%2520Edition.exe
https://gist.githubusercontent.com/CHEF-KOCH/2dea75d43b2184f228ae94b168d275b1/raw/35d7a4447a198449bbb3280e1c3d7a57517350de/Canvas%2520fingerprinting%2520pages%2520%255B2017%2520Edition%255D.exe
https://v.firebog.net/hosts/static/SamsungSmart.txt
https://v.firebog.net/hosts/Easyprivacy.txt
https://raw.githubusercontent.com/TakoYachty/Gift-Card-Killer/master/giftcardkiller.txt
https://raw.githubusercontent.com/WindowsLies/BlockWindows/master/hosts
http://s3.amazonaws.com/lists.disconnect.me/simple_tracking.txt
https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/fakenews-gambling-porn/hosts
```
## Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


[Back Home](https://plaintoast.org)
