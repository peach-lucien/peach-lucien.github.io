---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

My research deals with the analysis of complex systems that can be abstracted as networks or graphs. In particular, I work on applications and development of graph theoretical tools. On the theoretical front, I am exploring the connection between graph theory and machine learning, with a more recent focus on higher-order network structures. On the application front, my focus is in neuroscience but also dabble into healthcare and learning analytics.

Check out some of my projects below!

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}
