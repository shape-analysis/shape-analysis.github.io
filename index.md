---
layout: page
title: "Shape analysis"
description: "Mailing list and seminar"
background: "img/banner_4.png"
---


This website is home to the French research community on the **analysis of 3D shapes**, from biomedical imaging to computer assisted design and graphics.

We organize an **open seminar** in Paris and diffuse announcements related to relevant software tools, conferences and job offers.

Please feel free to invite newcomers in the field (interns, students, engineers...).

### Mailing list


To register to **shapes@inria.fr**, please:

1. Send a message with title "**subscribe shapes Your Name**" to **[sympa_inria@inria.fr](mailto:sympa_inria@inria.fr)**.
2. You will then receive an **invite link**. <span style="color:red">**Don't forget to click on it**</span>, or you won't be registered as a subscriber!

<br/>

### Shape seminar

Every three weeks, we organize an in-person seminar in Paris around noon:

  - 60mn of informal discussions, followed by a **30mn presentation**.
  - <span style="color:red">**Free lunch**</span> is provided by Barbara Gris thanks to an Emergence(s) grant of the Ville de Paris.
  - <span style="color:red">**Videos**</span> for most presentations will be available on YouTube.
  - <span style="color:red">**Registration**</span> **is free but mandatory [(click here)](https://forms.gle/vCJExSJDWaQiDitY7).**

<br/>

<hr>
{% for oneitem in site.data.seminar %}
   <h5>{{ oneitem.date }} &#8212; {{ oneitem.title }}</h5>
  <p>
  <b>Time: </b> {{ oneitem.time }}. <br/>
  <b>Location:</b> {{ oneitem.location | markdownify | remove: '<p>' | remove: '</p>' }}
  <div style="margin-bottom:0.5em;"></div> 
  <b>Speaker:</b> <a href="{{ oneitem.url }}">{{ oneitem.speaker }}</a>  ({{ oneitem.affiliation }}) 
  <div style="margin-bottom:0.5em;"></div> 
  <b>Abstract:</b> {{ oneitem.abstract | markdownify | remove: '<p>' | remove: '</p>'  }}
  </p>
  <hr>
{% endfor %}

<br/>

### Organizers

- [Barbara Gris](http://gris.perso.math.cnrs.fr/) (CNRS).
- [Benjamin Charlier](https://imag.umontpellier.fr/~charlier/index.php?page=index) (Université de Montpellier).
- [Jean Feydy](https://www.jeanfeydy.com/) (INRIA).
- [Joan Glaunès](https://helios2.mi.parisdescartes.fr/~glaunes/) (Université Paris-Cité).


### Sponsors

<p align="center">

<a href="https://www.sciencesmaths-paris.fr/">
<img width="150" src="../img/logo-fsmp.png"/>
</a>&nbsp;&nbsp;

</p>
