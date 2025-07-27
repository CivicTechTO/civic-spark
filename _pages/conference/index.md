---
layout: page
title: Conference | Overview
description: Saturday, August 16, 2025 – Talks, sessions, and shared lessons from the field.
permalink: /conference/
redirect_from: /conference
---

{% include conference-subnav.html%}

<article class="grid grid-blade ">
<div class="image-area colorized-magenta">
  {% include svg-converse.svg %}
</div>
<div class="text-area">
  <h2 class="colorized-magenta">Overview</h2>
<p><span class="lead">This isn’t a product pitch stage. It’s a space to <strong class="colorized-magenta">share real stories</strong>, <strong class="colorized-magenta">reflect on hard-won lessons</strong>, and <strong class="colorized-magenta">explore what’s possible</strong> when we build with care, creativity, and community.</span></p>
<p>The Civic Spark Conference kicks off with a curated day of panels, talks, and workshops — spotlighting the people building community-powered tools, services, and networks across North America.</p>
<p>You can expect:</p>
<ul>
<li>Lived experience, not just expertise</li>
<li>Reflections on practice, not polished narratives</li>
<li>Lessons from the field, not pitches</li>
<li>Space to listen, learn, and be inspired</li>
</ul>

</div>
</article>

<section>
<h2 class="colorized-magenta">Speakers</h2>
<div class="speaker-grid">
  {% assign shuffled_speakers = site.speakers | sample: 3 %}
  {% for speaker in shuffled_speakers %}
    {% include speaker-card.html speaker=speaker %}
  {% endfor %}
</div>
<p>See the full lineup and speaker details on the <a href="{{ '/conference/speakers' | relative_url }}">Speakers page</a>.</p>
</section>

<section>
<h2 class="colorized-magenta">Themes</h2>
<p>Our programming is organized around three guiding themes.</p>

<div class="grid">
  <article>
    <hgroup>
    <h3 class="colorized-magenta">Building Together</h3>
    <p>Community Based Innovation</p>
    </hgroup>
    <p><small>How do we co-create civic services, tools, or support networks from the ground up?</small></p>
    <p><small>Learn from community-led projects, grassroots collaboration, and the creative (often messy) process of making change happen.</small></p>
  </article>
  <article>
    <hgroup>
    <h3 class="colorized-magenta">Tech That Serves</h3>
    <p>Appropriate Tech</p>
    </hgroup>
    <p><small>How do communities use technology to achieve their own socially aligned outcomes?</small></p>
    <p><small>Go beyond the hype to focus instead on tools designed with and for community needs.</small></p>
  </article>
  <article>
    <hgroup>
    <h3 class="colorized-magenta">Intersections of Change</h3>
    <p>Collaborating Across Sectors</p>
    </hgroup>
    <p><small>How can communities, government, academia, and nonprofits be better together?</small></p>
    <p><small>Dig into the reality of cross-sector work — what helps, what hurts, and what’s possible.</small></p>
  </article>
</div>
</section>

## More

[View the Speakers]({{'/conference/speakers' | relative_url}}){:role="button"}{:class="outline"} [View the Schedule]({{'/conference/schedule' | relative_url}}){:role="button"}{:class="outline"} [Unconference page]({{'/unconference' | relative_url}}){:role="button"}{:class="secondary outline"}
