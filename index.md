---
layout: page
title: "Shape analysis"
description: "Mailing list and seminar"
background: "img/banner_4.png"
---


This website is home to the French research community on **shapes analysis**, from biomedical imaging to computer assisted design and graphics. 

We organize an **open seminar** in Paris and diffuse announcements related to relevant software tools, conferences and job offers. You may subscribe to the <a href="#mailing_list">mailing list</a>, feel free to invite newcomers in the field (interns, students, engineers...). You may also consider to subscribe to the <a href="#calendar_feed">calendar feed</a>. 

### Shape seminar

Every three weeks, we organize an in-person seminar in Paris around noon:

  - 60mn of informal discussions, followed by a **60mn presentation**.
  - you are welcome to share the free **lunch** that we provide.
  - **Videos** for most presentations are available on YouTube [(click here)](https://www.youtube.com/watch?v=m68NjYSD7gU&list=PLBFtqeJgRBGies4qp_XWlrsYxgDePEmtp).

<iframe width="560" height="315" src="https://www.youtube.com/embed/m68NjYSD7gU?si=a-Pvs-yTmxUVwgSq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br/>

{% for oneitem in site.data.seminar %}
  {% if oneitem.location %}
  <hr>
  {% endif %}

   <h5>{{ oneitem.date }} &#8212; {{ oneitem.title }}</h5>
  <p>

  <a href="{{ oneitem.url }}">{{ oneitem.speaker }}</a>  ({{ oneitem.affiliation }}) 
  
  {% if oneitem.time %}
  at <b>{{ oneitem.time }}</b>
  {% endif %}
  {% if oneitem.location %}
  in {{ oneitem.location | markdownify | remove: '<p>' | remove: '</p>' }}
  <!--<div style="margin-bottom:0.5em;"></div> -->
  {% endif %}

  {% if oneitem.video or oneitem.slides or oneitem.code or oneitem.registration %}
   <br/><!--<div style="margin-bottom:0.5em;"></div> -->
   <b>Links:</b> 
    {% if oneitem.video %}
      <a href="{{ oneitem.video }}"><b>video</b></a>
    {% endif %}
    {% if oneitem.slides %}
      <a href="{{ oneitem.slides }}">slides</a> 
    {% endif %}
    {% if oneitem.code %}
      <a href="{{ oneitem.code }}">code</a> 
    {% endif %}
    {% if oneitem.registration %}
      <a href="{{ oneitem.registration }}"><span style="color:red"><b>Registration</b></span></a> is free but mandatory.
    {% endif %}
  {% endif %}

   <!--<br/> <div style="margin-bottom:0.2em;"></div> -->
   <details>
   <summary><b>Abstract:</b></summary> 
   {{ oneitem.abstract | markdownify | remove: '<p>' | remove: '</p>'  }}
   </details>

  </p>
{% endfor %}
<hr>

<br/>

### <a id="mailing_list" />Mailing list


To register to **shapes@inria.fr**, please:

1. Send a message with title "**subscribe shapes Your Name**" to **[<span style="color:red">sympa_inria</span>@inria.fr](mailto:sympa_inria@inria.fr?subject=subscribe shapes)**.
2. You will then receive an **invite link**. <span style="color:red">**Don't forget to click on it**</span>, or you won't be registered as a subscriber!

<br/>

### <a id="calendar_feed" />Ical feed

A calendar feed of the seminar is available for subscription. Simply add this <a href="/shape-analysis-seminar.ics">ical link</a> to your calendar app.

<br/>

### Organizers

- [Benjamin Charlier](https://imag.umontpellier.fr/~charlier/) (Université de Montpellier).
- [Jean Feydy](https://www.jeanfeydy.com/) (INRIA).
- [Joan Glaunès](https://helios2.mi.parisdescartes.fr/~glaunes/) (Université Paris-Cité).
- [Barbara Gris](http://gris.perso.math.cnrs.fr/) (CNRS).


### Sponsors

<p align="center">

<img height="80" src="../img/paris.jpg"/>&nbsp;&nbsp;
<a href="https://www.sciencesmaths-paris.fr/">
<img height="80" src="../img/logo-fsmp.png"/>
</a>
</p>
