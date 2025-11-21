---
title: Projects
nav:
  order: 2
  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

Our projects bridge the gap between fundamental AI research and real-world applications. We develop intelligent systems that can predict, design and control complex phenomena across various domains, from molecular design to mechanical systems.

{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filter="group == 'featured'" style="large" %}

{% include section.html %}

## On Going

{% assign ongoing_projects = site.data.projects | where_exp: "project", "project.group != 'featured'" %}
{% capture ongoing_content %}
{% for project in ongoing_projects %}
  {% include card.html 
    title=project.title 
    subtitle=project.subtitle 
    image=project.image 
    link=project.link 
    description=project.description 
    tags=project.tags 
    style="large"
  %}
{% endfor %}
{% endcapture %}

{% include grid.html content=ongoing_content %}

{% include section.html %}
