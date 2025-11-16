---
layout: page
title: Articles
---

{% for article in site.articles %}
  {% assign a = article %}
  <div class="article-item" style="margin-bottom:40px;">

    <div style="display:flex; gap:20px; align-items:flex-start;">
      
      {% if a.thumbnail %}
      <div style="width:200px; min-width:200px;">
        <img src="{{ a.thumbnail }}" alt="{{ a.title }}" style="width:100%; border-radius:8px;">
      </div>
      {% endif %}

      <div>
        <h2 style="margin-top:0;">
          <a href="{{ a.link }}">{{ a.title }}</a>
        </h2>

        <p>{{ a.description }}</p>

        <div style="margin:10px 0;">
          {% for tag in a.tags %}
          <span style="
            background:#6c63ff;
            color:white;
            padding:4px 10px;
            border-radius:15px;
            font-size:12px;
            margin-right:5px;">
            {{ tag }}
          </span>
          {% endfor %}
        </div>

        <p style="font-size:13px; opacity:0.7;">
          Last updated: {{ a.last_updated }}
        </p>
      </div>

    </div>

  </div>
{% endfor %}
