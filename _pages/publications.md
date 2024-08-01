---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2>Methodological Research</h2>
{% for post in site.publications reversed %}
  {% if post.category == "methodological" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Applied Research</h2>
{% for post in site.publications reversed %}
  {% if post.category == "applied" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
