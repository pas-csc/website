---
layout: static
title: Events
markdown: kramdown
---
# Pasadena Complete Streets Coalition Events

Something about events.

{% for event in site.events %}
{{ event.title }}
{% endfor %}
<!--
<hr>
See our Google Calendar [(open in new window)](https://calendar.google.com/calendar/embed?src=e2951ldkd87chs8raacpep5648%40group.calendar.google.com&ctz=America%2FLos_Angeles) or add it to yours ([Android/Web](https://calendar.google.com/calendar?cid=ZTI5NTFsZGtkODdjaHM4cmFhY3BlcDU2NDhAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ), [iCal](https://calendar.google.com/calendar/ical/e2951ldkd87chs8raacpep5648%40group.calendar.google.com/public/basic.ics))

<!--Show on larger screens
<iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showNav=0&amp;showPrint=0&amp;showCalendars=0&amp;height=600&amp;wkst=1&amp;bgcolor=%23ffffff&amp;src=e2951ldkd87chs8raacpep5648%40group.calendar.google.com&amp;color=%2328754E&amp;ctz=America%2FLos_Angeles" style="border-width:0" width="800" height="600" frameborder="0" scrolling="no" class="d-none d-md-block"></iframe>

<!--Show on smaller screens
<iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;showTabs=0&amp;showCalendars=0&amp;mode=AGENDA&amp;height=600&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=e2951ldkd87chs8raacpep5648%40group.calendar.google.com&amp;color=%2328754E&amp;ctz=America%2FLos_Angeles" style="border-width:0" width="400" height="600" frameborder="0" scrolling="no" class="d-md-none"></iframe>


-->

{% include mailchimp.html %}