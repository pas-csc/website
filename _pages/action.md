---
layout: staticalerttarget
title: 'Action Alert: Support Our Growing Bicycle Network!'
markdown: kramdown
---

Updated May 10, 2019.

# Do you want safer streets? Would you like to comfortably ride a bike, skateboard, scooter, or other wheeled device in Pasadena?

If your answer is "yes"...

# SUPPORT FUNDING FOR PASADENA'S BICYCLE NETWORK! 

## Here are {{ site.actionitems.size }} simple actions you can take to ensure that an accessible network of walk/bike/skate+ friendly projects is installed in Pasadena:
 
{% for item in site.actionitems %}
{% if item.linkURL %}
<h3 style="color:#91c346"><a href="{{ item.linkURL }}">{{ item.title }}</a></h3>
{% else %}
<h3 style="color:#91c346"> {{ item.title }}</h3>
{% endif %}

<!---<img src="{{ item.imgURL }}" class="img-fluid" style="padding:5px;"><br>--->
{{ item.content }}
{% endfor %}
 
### Thank you for standing up for safe streets! If you'd like to keep in touch, please consider signing up for monthly updates below.

{% include mailchimp.html %}