---
title: Organisers
layout: single
sidebar: 
  nav: "people"
permalink: /people/
classes: wide
---

The themester is jointly organised by organisers supported by staff. Each individual event listed on the [upcoming events]({% link recent.md %}) page listing specific programme or workshop organisers.


<ul id="profiles">
  {% assign sorted = site.members | sort: 'last'  %}
  {% for member in sorted %}
    <li >
      <div class="row">
        <div class="column1">
           <a href="{{ member.homepage }}">
           <img  src="/assets/pics/{{member.pic}} " id="two_col_img"/></a>
        </div>
        <div class="column2">
        {% if member.homepage %}
        <a class="btn btn--inverse" href="{{ member.homepage }}"> {{member.given}} {{ member.last}} </a>
        {% else %}
        <span class="btn btn--inverse"> {{member.given}} {{ member.last}} </span>
        {% endif %}
        {% if member.email %}
        <a class="btn btn--inverse" href="mailto:{{ member.email }}"> Email </a>
        {% endif %}
        <p class="small">{{ member.research | markdownify | remove: "<p>" | remove: "</p>" }}</p>
       </div>
      </div>
    </li>
  {% endfor %}
</ul>
 