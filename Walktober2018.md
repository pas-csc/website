---
layout: static-info
title: Walktober 2018 with Pasadena CSC
---
<div class="container" id="pagetop" style="padding-top:30px;">
  <div class="row"> 
    <div class="col">
      <h1 class="display-4 text-center">Walktober 2018<br>A Celebration of Walking in Pasadena</h1>
    </div>
  </div>
  
  <div class="row"> 
    <div class="col">
      <h3 class="text-center">Presented by the Pasadena Complete Streets Coalition and Day One</h3> 
      <p class="text-center"><img class="walklogo" src="{{ site.url }}/img/csc_logos/banner_small.jpg" width="300px" alt="Pasadena CSC" style="margin:0em 1.5em;"><img src="{{ site.url }}/img/walktober/dayone-logo.jpg" width="150px" alt="Day One" style="margin:0em 1.5em;"></p>
      <h3 class="text-center">in collaboration with:</h3>
      <p class="text-center"><img src="{{ site.url }}/img/walktober/artwalk-logo.png" width="200px" alt="Pasadena ArtWalk"> 
      <img src="{{ site.url }}/img/walktober/opmd-logo.jpg" width="200px" alt="Old Pasadena Management District">
      <img src="{{ site.url }}/img/walktober/pasadenaheritage-logo.jpg" width="200px" alt="Pasadena Heritage">
      <img src="{{ site.url }}/img/walktober/pwt-logo.png" width="100px" alt="Pasadena Walking Tours"> 
      <img src="{{ site.url }}/img/walktober/jaycees-logo.jpg" width="100px" alt="Pasadena Jaycees"> 
      <img src="{{ site.url }}/img/walktober/club21-logo.jpg" width="200px" alt="Club 21"><br>
      Pasadena Downtown Neighborhood Association, Pasadena Water and Power, and Pasadena Citizen's Service Center</p>
    </div>
  </div>
</div>

<!--Poster-->
<div class="container" style="padding-top:30px;">
  <div class="row">
    <div class="col text-center"><img src="{{ site.url }}/img/walktober/walktober.jpg" class="img-fluid"></div>  
  </div>
  <div class="row">
      <div class="col text-center"><p><em>Poster credit: Adrian Kalvinskas, <A href="https://distantlandsblog.wordpress.com/" target="_blank" rel="noopener noreferrer">Distant Lands Pasadena</a></em></p></div>  
  </div>
</div>

<!--Calendar-->
<div class="container" style="padding-top:30px;">
<h1>Calendar of Events</h1>
<p class="lead"><em>All dates are in October.</em></p>

{% for event in site.data.walkList %}
<div class="card card-body mb-3">
  <div class="row">
    <div class="col">
        <div class="datebox float-left">{{ event.Day }}<br>{{ event.Date }}</div>
        <h2>{{ event.Name }}</h2>
        <div class="row">
            <div class="col-auto"><p><i class="far fa-clock"></i> {{ event.Time }}</p></div>
            <div class="col-auto"><p><i class="fas fa-dollar-sign"></i> {{ event.Price }}</p></div>
            <div class="col-auto"><p><i class="fas fa-map-marker-alt"></i> {{ event.Meet }}</p></div>
        </div>
        <p><a data-toggle="collapse" href="#{{ event.Name | slice:0,3 }}-{{ event.Date }}-col" role="button" aria-expanded="false" aria-controls="{{ event.Name | slice:0,3}}-{{ event.Date }}-col">Details</a> | <a href="{{ event.Page }}" target="_blank" rel="noopener noreferrer">{{ event.PageType }}</a></p>
            <div class="collapse" id="{{ event.Name | slice:0,3 }}-{{ event.Date }}-col">
                {% if event.Detail1 != nil %}<p>{{ event.Detail1 }}</p>{% endif %}
                {% if event.Detail2 != nil %}<p>{{ event.Detail2 }}</p>{% endif %}
                {% if event.Partner =="Y" %}<p>This is a partner event, so please see our partner's <a href="{{ event.Page }}" target="_blank" rel="noopener noreferrer">event page</a> for the most up-to-date information.</p>{% endif %}
                <p><em>Hosted by <a href="{{ event.Org1Site }}" target="_blank" rel="noopener noreferrer">{{ event.Org1 }}</a>{% if event.Org2 != nil %} and <a href="{{ event.Org2Site }}" target="_blank" rel="noopener noreferrer">{{ event.Org2 }}</a>{% endif %}</em>.</p>
    </div>
    </div> 
  </div>
</div>
{% endfor %}
  
</div>

# About Walktober

Press release info goes here
# Proclamation

Blurb about proclamation

# About PasadenaCSC

Blurb about us, [link to main site]({{ site.url }})