---
layout: single
title: Events
permalink: /events/index.html
sidebar: 
  nav: "events"
classes: wide
---

Activities taking place as part of the Environmental and Climate Resilience themed semester.

<ul id="two_col">
  <li>
    <div class="column2">
      <a class="btn btn--inverse" href="{{ '/events/current_seminars.html' | relative_url }}">Seminars</a>
      <p class="small">Weekly seminars on the theme, hosted throughout the semester.</p>
    </div>
  </li>
  <li>
    <div class="column2">
      <a class="btn btn--inverse" href="https://imibath.ac.uk/2026/06/02/power-of-3/">Power of 3 workshop</a>
      <p class="small">17 September 2026 &mdash; form cross-faculty collaborations and secure funding for early-stage research ideas.</p>
    </div>
  </li>
  <li>
    <div class="column2">
      <a class="btn btn--inverse" href="{{ '/events/hydrology-workshop.html' | relative_url }}">Hydrology workshop</a>
      <p class="small">Details to be announced.</p>
    </div>
  </li>
</ul>

### Recent posts

<ul>
{% for post in site.posts limit: 3 %}
  <li><a class="btn btn--inverse" href="{{site.url}}{{site.baseurl}}{{post.url}}">  {{post.title}}
  </a>
  <div class="small"> {{post.excerpt}}
  </div></li>
{% endfor %}
</ul>
