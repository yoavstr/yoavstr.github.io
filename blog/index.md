---
layout: default
title: Blog
---

## My Posts

{% for post in site.posts %}
* **{{ post.date | date: "%B %d, %Y" }}** — [{{ post.title }}]({{ post.url | relative_url }})
  <br>_{{ post.description | default: "No description provided." }}_
{% else %}
  There are no posts yet. Stay tuned!
{% endfor %}

---
[← Back Home]({{ '/' | relative_url }})