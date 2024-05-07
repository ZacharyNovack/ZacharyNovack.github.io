---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if author.googlescholar %} -->

<!-- {% endif %} -->

{% include base_path %}

You can also find my articles on my <a href="https://scholar.google.com/citations?user=fZKJdb0AAAAJ&hl=en&authuser=2">Google Scholar</a> profile.

**Preprints**
{% for post in site.publications reversed %}
  {% if post.pub_status == 'preprint' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

**Conference Publications**
{% for post in site.publications reversed %}
  {% if post.pub_status == 'conference' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

**Workshop Publications**
{% for post in site.publications reversed %}
  {% if post.pub_status == 'workshop' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

**Non Refereed Publications**
{% for post in site.publications reversed %}
  {% if post.pub_status == 'nonrefereed' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}