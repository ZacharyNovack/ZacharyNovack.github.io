---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if author.googlescholar %} -->

<!-- {% endif %} -->

{% include base_path %}

You can also find my articles on my <u><a href="https://scholar.google.com/citations?user=fZKJdb0AAAAJ&hl=en&authuser=2">Google Scholar</a> profile.</u>

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<sup>*</sup> Equal authorship