---
layout: default
title: 
permalink: /publications/

---

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

