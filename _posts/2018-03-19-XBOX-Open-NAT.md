---
layout: default
title: "XBOX Open NAT"
comments: true
categories: pfsense
---
[Home](https://plaintoast.org) - [pfsense](https://plaintoast.org/pfsense.html)

# Quick and Easy XBOX Open NAT Guide

Open NAT for XBOX behind pfsense requires either port triggering or port forwarding to obtain open NAT. This is a quick guide on how to obtain open NAT while limiting UPnP to only your XBOX. This guide also applies to other devices Playstation or the Nintendo Switch.   

## Create Static IP

```staticIP
1) Login to pfsense and navigate to Status/DHCP Leases
2) Select the white plus box (you should see "add static mapping" on hover
3) Enter your static IP
4) Save
``` 

## ENABLE UPnP

```upnp
1) Navigate to Services/UPnP & NAT-PMP
2) Select "Enable" and "UPnP Port Mapping"
3) Select "Default Deny"
4) Add the following ACL Entries: allow 53-65535 192.168.1.200/32 53-65535 
5) Save
``` 

## Add NAT Rule

```NAT
1) Navigate to Firewall/NAT/Outbound
2) Change outbound NAT Mode to Hybrid 
3) Select add new mapping
4) Add XBOX static IP (or alias if created) to Source field
5) Select Static Port under Translation - Port or Range
5) Save
``` 

## Restart XBOX
```xboxr
1) Power on your XBOX
2) Navigate to "Restart" and select
3) Navigate to "Network Settings" to identify NAT type
```
### Success!

At this point you should have open NAT on your XBOX using UPnP that is restricted to the XBOX. Enjoy!!! 

**Please let me know if I missed something or could improve this solution in the comments below.**

<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://plaintoast.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>

## Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
