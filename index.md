---
layout: default
title: Camille Eckert
---

## About Me


![Profile Picture]({{ "assets/images/Profile-photo.jpg" | relative_url }}){: class="profile-image"}

 
My name is Camille. I am a sophomore mechanical engineer at Cornell University.

Take a look at <a href="{{ "/projects/" | relative_url }}">my projects</a> or my <a href="{{ "/cv/" | relative_url }}">CV</a>.

{% assign actuator = site.projects | where: "title", "ENGRD-2020-Actuator Design" | first %}
{% if actuator %}
Jump directly to my <a href="{{ actuator.url | relative_url }}">{{ actuator.title }}</a> project.
{% endif %}

## Featured Projects

<div class="gallery-container">
<div class="project-gallery">
  {% for project in site.projects %}
    <div class="gallery-item">
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
        <p>{{ project.title }}</p>
      </a>
    </div>
  {% endfor %}
</div>
</div>
