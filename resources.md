---
layout: page
title: Resources
permalink: /resources/
---

## Educational Resources

Access our collection of educational materials, publications, and tools for learning about renewable energy.

### Learning Materials

[Content to be added based on actual website content]

### Publications

<div class="resources-grid">
    {% for publication in site.publications %}
    <div class="resource-card">
        <h3><a href="{{ publication.url | relative_url }}">{{ publication.title }}</a></h3>
        {% if publication.date %}
        <p><em>{{ publication.date | date: "%B %Y" }}</em></p>
        {% endif %}
        {% if publication.excerpt %}
        <p>{{ publication.excerpt }}</p>
        {% endif %}
    </div>
    {% endfor %}
</div>

### Downloads

[Content to be added based on actual website content]

### External Links

[Content to be added based on actual website content]
