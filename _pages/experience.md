---
permalink: /experiences/
title: "Experiences"
---

<div class="experience-grid">
{% for exp in site.data.experiences %}
  <a href="{{ exp.link | relative_url }}" class="experience-card">
    <div class="logo-wrap">
      <img src="{{ exp.logo | relative_url }}" alt="{{ exp.company }} logo" loading="lazy" />
    </div>
    <div class="experience-content">
      <div class="experience-header">
        <h3 class="company">{{ exp.company }}</h3>
        <span class="dates">{{ exp.dates }}</span>
      </div>
      <p class="title">{{ exp.title }}</p>
      <p class="description">{{ exp.description }}</p>
    </div>
  </a>
{% endfor %}
</div>
