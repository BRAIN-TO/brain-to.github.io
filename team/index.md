---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our interdisciplinary team of researchers, engineers, and clinicians is dedicated to advancing the field of neuroimaging and improving patient care. We bring together expertise from various domains to foster innovation and collaboration in our research endeavors. The team includes postdoctoral fellows, graduate students, research assistants, and administrative staff, all working together to achieve our mission. We also work closely with collaborators from other institutions and industry partners to enhance our research impact.

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'principal investigator'" %}
{% include list.html data="members" component="portrait" filter="role == 'postdoc' and group != 'alum'" %}
{% include list.html data="members" component="portrait" filter="role == 'phd' and group != 'alum'" %}
{% include list.html data="members" component="portrait" filter="role == 'msc' and group != 'alum'" %}
{% include list.html data="members" component="portrait" filter="role == 'staff' and group != 'alum'" %}
{% include list.html data="members" component="portrait" filter="role == 'undergrad' and group != 'alum'" %}

{% comment %}
If you are interested in joining our team, please visit our [Join Us](/careers) page for current openings and application instructions.
{% endcomment %}


{% include section.html background="images/background_dark.jpg" dark=false %}

# Alumni

{% include section.html %}

{% capture content %}

{% include list.html data="members" component="portrait" filter="group == 'alum'" style="small" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
