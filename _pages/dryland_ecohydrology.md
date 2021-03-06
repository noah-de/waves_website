---
layout: splash
permalink: /dryland_ecohydrology/
title: "Dryland Ecohydrology"
author_profile: false
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/dryland_ecohydrology.jpg
excerpt: 'Characterizing the structure and function of water-limited landscapes.'
tags:
    - Dryland Ecohydrology
---

{% include group-by-array collection=site.posts field="tags" %}

Our drylands research is focused on understanding how rainfall variability affects ecosystem processes and the provision of ecosystem services. We are particulary interested in understand the critical role that coupled spatial patterns of plants, soils, and resources play in determining the dynamics and resilience of dryland ecosystems. Our work in these areas seeks to combine field observations, computational modeling, and development of new concepts and theories.

## News and Updates:

{% for tag in page.tags %}
    {% for post in site.posts %}
        {% if post.tags contains tag %}
            {% include archive-single.html %}
        {% endif %}
    {% endfor %}
{% endfor %}

