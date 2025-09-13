---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

At the AiRA Lab, we believe that great research begins with respect and collaboration. Our team is built on a foundation of curiosity, shared knowledge, and the drive to make meaningful contributions to science and technology. Together, we explore new ideas and encourage one another to grow, creating an environment where innovation can truly flourish.

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'pi'" %}
{% include list.html data="members" component="portrait" filter="role != 'pi'" %}

{% include section.html background="images/background.jpg" dark=true %}

Beyond individual achievements, we value the collective spirit that unites us. Every project we pursue is guided by inspiration and the desire to make a positive impact on society. By working together and supporting each other, we aim to push the boundaries of discovery and leave behind research that matters.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
