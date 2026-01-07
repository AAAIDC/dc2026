---
layout: page
title: Panelists
permalink: "/panelists/"
---

{% for speaker in site.panelists %}
  <div class="speaker">
     <p>
     <h2>{{ speaker.name }}</h2> 
     <center>
    {{ speaker.role }}, &nbsp;  {{ speaker.institution }} &nbsp; <a href="{{ speaker.website }}"> Homepage </a> </center> <br>
    <p class="aligncenter">
             <img src="{{ speaker.image }}" alt="{{ speaker.image }}" style="max-height:250px;">
    </p>
    </p>
    <p><b>Bio</b>: {{ speaker.bio }}</p>
  </div>
{% endfor %}
