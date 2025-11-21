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

## Recent Activities

Stay updated with our latest project developments, conference presentations, and research milestones. Our team actively participates in international conferences and collaborates with research institutions worldwide.

### Conference Presentations
- **ICEMA-25 Conference** (November 2025) - Presented research on origami dynamics, flexible systems modeling, and control theory at Vietnam National University, Hanoi
- **International Symposium on Computational Mechanics** - Showcasing AI-driven approaches to mechanical system design

### Research Milestones
- Advanced modeling frameworks for flexible robotic systems
- Novel origami-inspired structural designs for deployable applications
- Integration of machine learning with traditional mechanical engineering approaches

{% include section.html %}

## Publications & Resources

Our research contributes to the scientific community through peer-reviewed publications, open-source software, and educational resources.

### Recent Publications
{% include list.html data="citations" component="citation" style="rich" filter="tags.to_s.include?('project')" %}

### Open Source Projects
- Computational tools for origami design and simulation
- Machine learning frameworks for robotic control
- Educational resources for AI in mechanical engineering

### Datasets & Resources
- Origami folding pattern databases
- Flexible system dynamics datasets
- Benchmark problems for AI-driven control systems
