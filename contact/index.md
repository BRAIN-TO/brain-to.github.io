---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Our lab is proudly supported by the [University Health Network (UHN)](http://www.uhn.ca), [Sunnybrook Research Institute (SRI)](https://research.sunnybrook.ca/), and the [University of Toronto (UofT)](https://www.utoronto.ca/). We are based in various locations across Toronto, Canada depending on the project and collaboration. For general inquiries, please contact us using the information below.

{%
  include button.html
  type="email"
  text="Kamil.Uludag@uhn.ca"
  link="Kamil.Uludag@uhn.ca"
%}
{%
  include button.html
  type="phone"
  text="(416) 603-2581"
  link="+14166032581"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  text="Toronto Western Hospital"
  link="https://maps.app.goo.gl/j5WHBVV1xoQMjpzK9"
%}

{% include section.html %}

# Sponsors & Partners

{% capture col1 %}

{%
  include figure.html
  image="images/cfi.png"
%}

{%
  include figure.html
  image="images/slaight.jpg"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/crc.jpg"
%}

{%
  include figure.html
  image="images/koerner.png"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

# Visit Us

As an interdisciplinary lab, we have offices at multiple UHN sites. You will find us here:

{% capture col1 %}
Techna Institute

101 College Street, Princess Margaret Cancer Research Tower
7th Floor, Room 7-208
Toronto, ON, Canada, M5G 1L7

{% endcapture %}

{% capture col2 %}
Toronto General Hospital

200 Elizabeth Street, 
BPMB 160 (B-Floor, Peter Munk Building),
Toronto, ON, Canada, M5G 2C4

{% endcapture %}

{% capture col3 %}
Toronto Western Hospital

399 Bathurst Street,
12MC405 (12th floor, MacLaughlin Elevators),
Toronto, ON, Canada, M5T 2S8

{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
