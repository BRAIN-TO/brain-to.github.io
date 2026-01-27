---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Our lab is proudly supported by the [University Health Network (UHN)](http://www.uhn.ca), [Sunnybrook Research Institute (SRI)](https://research.sunnybrook.ca/), and the [University of Toronto (UofT)](https://www.utoronto.ca/). We are based in various locations across Toronto, Canada depending on the project and collaboration. For general inquiries, please contact us.

{%
  include button.html
  type="email"
  text="Kamil.Uludag@uhn.ca"
  link="Kamil.Uludag@uhn.ca"
%}

{% comment %}
{%
  include button.html
  type="phone"
  text="(416) 603-2581"
  link="+14166032581"
%}
{% endcomment %}

{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  text="Toronto Western Hospital"
  link="https://maps.app.goo.gl/j5WHBVV1xoQMjpzK9"
%}

{% include section.html %}

# Sponsors & Partners
{% capture content %}

{%
  include figure.html
  image="images/uhn.svg"
  height="200px"
%}

{%
  include figure.html
  image="images/koerner.png"
  height="200px"
%}

{%
  include figure.html
  image="images/slaight.jpg"
  height="200px"
%}

{%
  include figure.html
  image="images/cfi.png"
  height="200px"
%}

{%
  include figure.html
  image="images/nserc.png"
  height="200px"
%}

{%
  include figure.html
  image="images/shsc.svg"
  height="200px"
%}

{%
  include figure.html
  image="images/crc.jpg"
  height="200px"
%}

{% endcapture %}

{% include grid.html content=content %}

{% include section.html dark=true %}

# Visit Us

As an interdisciplinary lab, we have offices at various sites. You will find us here:

{% capture col1 %}
Princess Margaret Cancer Research Tower

101 College Street,
7th Floor, Room 7-208,
Toronto, ON, Canada, M5G 1L7

{% endcapture %}

{% capture col2 %}
Toronto Western Hospital

399 Bathurst Street,
12MC405 (12th floor, McLaughlin Elevators),
Toronto, ON, Canada, M5T 2S8

{% endcapture %}

{% capture col3 %}
Sunnybrook Research Institute

2075 Bayview Avenue,
EG 01 (E-wing, ground floor),
Toronto, ON, Canada, M4N 3M5

{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
