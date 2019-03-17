# Welcome to Plaintoast.org

You can expect to find random content, at random times, on this site. Content focuses on IT and security, but will also touch on other topics of interest. Feel free to bookmark, contribute, or [email me](mailto:ZcatK@plaintoast.org) your suggestions/feedback. 

## Topics

- [pfSense](/pfSense.html) - pfSense is a free and open source firewall and router that also features unified threat management, load balancing, multi WAN, and more.
- - [Python](/python.html) - An interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, Python has a design philosophy that emphasizes code readability, notably using significant whitespace. It provides constructs that enable clear programming on both small and large scales.
- *Coming Soon...*

## Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
