---
layout: default
title: Mehmet Cagri Altindal
---

<div class="profile-card">
  <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Profile">

  <h1>Mehmet Cagri Altindal</h1>
  <p class="title">PhD Candidate | Engineering Cybernetics, NTNU</p>

  <div class="social-links">
    <a href="https://www.linkedin.com/in/mehmet-cagri-altindal-15727829/"><i class="fa fa-linkedin-square fa-2x"></i></a>
    <a href="https://github.com/mehmetcaltindal"><i class="fa fa-github-square fa-2x"></i></a>
    <a href="https://scholar.google.com/citations?user=YqhyGVIAAAAJ&hl=en" target="_blank" aria-label="Google Scholar">
    <i class="fa fa-graduation-cap fa-2x"></i>
    </a>
    <a href="mailto:mcagrialtindal@gmail.com"><i class="fa fa-envelope fa-2x"></i></a>
  </div>
</div>


<div class="card">
  <h2>About</h2>
  <p>
    My research focuses on developing anomaly detection algorithms, real-time online calibration of drilling hydraulics models using both surface and downhole measurements to enhance drilling efficiency and hole cleaning management. My work combines adaptive learning, machine learning, drilling data and first-principal models to build robust hybrid modeling approaches for real-time applications. 
  </p>
</div>


<div class="card">
  <h2>Publications</h2>

  <ul class="pub-list">
    {% for pub in site.data.publications %}
      <li class="pub-item">
        <strong>{{ pub.title }}</strong><br>
        <span class="pub-authors">{{ pub.authors }}</span><br>
        <em>{{ pub.venue }}</em>, {{ pub.year }}
        {% if pub.link %}
          · <a href="{{ pub.link }}" target="_blank">link</a>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
</div>
