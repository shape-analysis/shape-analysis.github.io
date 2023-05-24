---
layout: page
title: "Shape analysis"
description: "A research community"
background: "img/paris1.png"
---


This website (under construction) is home to the French research community on the **analysis of 3D shapes**, from medical imaging to computer graphics and computer assisted design.
We organize an **open seminar** in Paris and diffuse announcements related to relevant software tools, conferences and job offers.

Please feel free to send an invitation to newcomers in the field (interns, students, engineers...).

Mailing list
-------------

To register to **shapes@inria.fr**, please:

1. Send a message with title "**subscribe shapes Your Name**" to **[sympa_inria@inria.fr](mailto:sympa_inria@inria.fr)**.
2. You will then receive an **invite link**.
3. <span style="color:red">**Don't forget to click on it**</span>, or you won't be registered as a subscriber!


Shape seminar
---------------

Every three weeks, we organize

**Registration is free but mandatory [(click here)](http://www.ihp.fr/en/CEB/T1-2019)** to let us order an adequate amount of food for the buffet.


<span style="color:red">**Videos for most presentations will be available on YouTube.**</span> 

{% for oneitem in site.data.seminar %}
<p>
   <b>{{ oneitem.date }}</b>, {{ oneitem.time }}.<br/>
  {{ oneitem.location | markdownify | remove: '<p>' | remove: '</p>' }}<br/>
  <a href="{{ oneitem.url }}">{{ oneitem.speaker }}</a>  ({{ oneitem.affiliation }})<br/>
  <b>Title:</b> <i>{{ oneitem.title }}</i><br/>
  <b>Abstract:</b> {{ oneitem.abstract | markdownify | remove: '<p>' | remove: '</p>'  }}
  </p>
{% endfor %}



Organizers
-----

- [Barbara Gris](http://gris.perso.math.cnrs.fr/) (CNRS).
- [Benjamin Charlier](https://imag.umontpellier.fr/~charlier/index.php?page=index) (Université de Montpellier).
- [Jean Feydy](https://www.jeanfeydy.com/) (INRIA).
- [Joan Glaunès](https://helios2.mi.parisdescartes.fr/~glaunes/) (Université Paris-Cité).


Sponsors
-----

<p align="center">

<a href="https://www.sciencesmaths-paris.fr/">
<img width="150" src="../img/logo-fsmp.png"/>
</a>&nbsp;&nbsp;

</p>
