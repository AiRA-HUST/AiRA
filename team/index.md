---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

At the AiRA Lab, we believe that great research begins with respect and collaboration. Our team is built on a foundation of curiosity, shared knowledge, and the drive to make meaningful contributions to science and technology. Together, we explore new ideas and encourage one another to grow, creating an environment where innovation can truly flourish.

{% include section.html %}

<!-- All Team Members in One Row -->
{% capture all_members_content %}
{% for member in site.members %}
  {% include portrait.html lookup=member.slug style="grid" %}
{% endfor %}
{% endcapture %}

{% include grid.html content=all_members_content style="team" %}

{% include section.html background="images/background.jpg" dark=true %}

Beyond individual achievements, we value the collective spirit that unites us. Every project we pursue is guided by inspiration and the desire to make a positive impact on society. By working together and supporting each other, we aim to push the boundaries of discovery and leave behind research that matters.

{% include section.html %}
