---
layout: static
title: Projects
markdown: kramdown
---
# Pasadena Complete Streets Coalition Projects

The projects highlighted below are only a small sampling of the work we do. Check back as we update this page...

{% for project in site.projects %}

<h2 style="padding-top:1.5em;"><a href="{{ project.linkURL }}">{{ project.title }}</a></h2>
<img src="{{project.imgURL}}" class="img-fluid" style="padding:5px;"><br>

{{ project.content }}

{% endfor %}

{% include mailchimp.html %}