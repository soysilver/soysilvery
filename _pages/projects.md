---
title:
layout: default
permalink: /projects/
published: true
---


<div class="ProjectContainer">

	<div class="gallery">


  {% for project in site.projects %}

  {% if project.redirect %}
  <div class="projectTile">
          <a href="{{ project.redirect }}" target="_blank">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
              <p>{{ project.description }}</p>
          </span>
          </a>
  </div>

  {% else %}

  <div class="projectTile">
          <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        	<div>
			{% if project.image %}
              			<img src ="{{project.image | prepend: site.baseurl}}">
			{% endif %}
        		<h3>{{ project.title }}</h3><br/>
              		<!--<p>{{ project.description }}</p>-->
          	</div>
          </a>
  </div>

  {% endif %}

  {% endfor %}

	</div>

</div>
