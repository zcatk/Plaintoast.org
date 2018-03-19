{% include head.html %}
# Welcome to Plaintoast.org

You can expect to find random content, at random times, on this site. Content focuses on IT and security, but will also touch on other topics of interest. Feel free to bookmark, contribute, or [email me](mailto:ZcatK@plaintoast.org) your suggestions/feedback. 

## Topics

- [pfsense](/pfsense.html) - pfSense is a free and open source firewall and router that also features unified threat management, load balancing, multi WAN, and more.
- *Coming Soon...*
- *Coming Soon...*

## Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
