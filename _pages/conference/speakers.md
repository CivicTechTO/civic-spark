---
layout: page
title: Conference | Speakers
description: Saturday, August 16, 2025 – Talks, sessions, and shared lessons from the field.
permalink: /conference/speakers/
---

{% include conference-subnav.html%}

<div class="speaker-grid">
  {% assign sorted_speakers = site.speakers | sort: "lastname" %}
  {% for speaker in sorted_speakers %}
    {% include speaker-card.html speaker=speaker %}
  {% endfor %}
</div>
