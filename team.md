---
layout: page
title: Team
permalink: /team/
---

## Our Team

Meet the people behind EduGrid who are dedicated to renewable energy education.

<div class="team-grid">
    {% for member in site.team %}
    <div class="team-card">
        {% if member.image %}
        <img src="{{ member.image | relative_url }}" alt="{{ member.name }}" class="team-photo">
        {% endif %}
        <h3><a href="{{ member.url | relative_url }}">{{ member.name }}</a></h3>
        {% if member.role %}
        <p class="role">{{ member.role }}</p>
        {% endif %}
        {% if member.excerpt %}
        <p>{{ member.excerpt }}</p>
        {% endif %}
    </div>
    {% endfor %}
</div>

## Collaborators

[Content to be added based on actual website content]

## Advisory Board

[Content to be added based on actual website content]
