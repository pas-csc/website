---
layout: staticalerttarget
title: 'Action Alert: Support the Union Street Protected Bike / Roll Lane!'
markdown: kramdown
---
# Do you want safer streets? Would you like to comfortably ride a bike, skateboard, scooter, or other wheeled device in Pasadena?

If your answer is "yes"...

# SUPPORT THE UNION STREET PROTECTED BIKE / ROLL LANE! 

## Here are three simple actions you can take to support the Union St. PBL and other walk/bike/skate+ friendly projects in Pasadena:
 
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