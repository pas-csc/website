---
layout: staticnoalert
title: 'Action Alert: Support Bus Rapid Transit and Our Bicycle Network!'
markdown: kramdown
---

Updated July 26, 2019.

# Do you believe the future of transportation in Pasadena and LA should be multi-modal?

If your answer is "yes"...

## Here are {{ site.actionitems.size }} simple actions you can take to be the change:
 
{% for item in site.actionitems %}
{% if item.linkURL %}
<h3 style="color:#91c346"><a href="{{ item.linkURL }}">{{ item.title }}</a></h3>
{% else %}
<h3 style="color:#91c346"> {{ item.title }}</h3>
{% endif %}

<!---<img src="{{ item.imgURL }}" class="img-fluid" style="padding:5px;"><br>--->
{{ item.content }}
<hr>
{% endfor %}
 
### Thanks for standing up for multi-modal transportation and safe streets! If you'd like to keep in touch, please consider signing up for monthly updates below.

{% include mailchimp.html %}