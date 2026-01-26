---
layout: page
title: News & Updates
subtitle: Latest from the EduGrid Project
---

## Recent News

Stay updated with the latest developments, announcements, and achievements from the EduGrid project.

<div class="card-grid">
  {% for post in site.posts limit:6 %}
  <div class="card">
    {% if post.image %}
    <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="card-image">
    {% endif %}
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
    <a href="{{ post.url | relative_url }}" class="btn btn-primary">Read More</a>
  </div>
  {% endfor %}
</div>

## All Posts

<div class="post-list">
  {% for post in site.posts %}
  <article class="post-item">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
      {% if post.author %} • by {{ post.author }}{% endif %}
    </p>
    <p>{{ post.excerpt | strip_html }}</p>
    {% if post.tags %}
    <div class="post-tags">
      {% for tag in post.tags %}
      <span class="tag">{{ tag }}</span>
      {% endfor %}
    </div>
    {% endif %}
  </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
<div class="text-center">
  <p>No news posts yet. Check back soon for updates!</p>
</div>
{% endif %}

---

## Subscribe to Updates

Want to stay informed about EduGrid news and developments? [Contact us]({{ '/contact' | relative_url }}) to subscribe to our newsletter.
