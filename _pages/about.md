---
layout: page
title: About Us
permalink: /about-us/
redirect_from: /about-us
---

<section>
  <article class="yellow-card-bg grid-blade">
    <div class="image-area">
      {% include svg-puzzle.svg %}
    </div>
    <div class="text-area">
      <h2>People Powered</h2>
      <p>Civic Spark is a people-organized gathering created by volunteers from Toronto who believe in building together – across roles, sectors, and lived experience.</p>
      <p>We’re designers, developers, public servants, organizers, and community builders who care deeply about how technology, data, and design can serve the public good.</p>
      <p>This isn’t a corporate event — it’s a collaborative effort grounded in care, curiosity, and community. We’re here to hold space for real stories, meaningful relationships, and the hard, hopeful work of civic action.</p>
    </div>
  </article>
</section>

## Our Why

<p class="lead">We envision a vibrant, people-centered civic ecosystem where communities use technology, organizing, and design to tackle real-world challenges — collaboratively, equitably, and creatively.</p>

For us Civic Spark is a space to:

- Spark new relationships, ideas, and actions.
- Bridge disciplines and sectors.
- Celebrate what’s working, and name what’s not.
- Push the civic tech movement forward — with values at the core.

<style>
.partner-lists{
  display: grid; 
  gap: 1rem; 
  grid-template-columns: 1fr;
  }
.partner-logo{height: 4rem; object-fit: contain;filter: grayscale(100%);}
@media (max-width: 767px) {
  .partner-logos {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>

<div class="organizing-partners">
  <h3>Civic Spark is organized by</h3>
  <div class="partner-lists">
    {% for sponsor in site.data.sponsors %}
      {% if sponsor.level == "organizing_partner" %}
        <div class="organizing-partner">
          <h4>{{ sponsor.title }}</h4>
          <a href="{{ sponsor.url }}" target="_blank" rel="noopener noreferrer" title="{{ sponsor.title }}">
            <img src="{{ site.baseurl }}/assets/images/sponsors/{{ sponsor.logo }}" alt="{{ sponsor.title }}" class="partner-logo">
          </a>
          {{ sponsor.description }}
        </div>
      {% endif %}
    {% endfor %}
  </div>
</div>
