---
permalink: /
title: "Lost in statistics"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---


---

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% include archive-single.html %}
{% endfor %}
