---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
classes: wide
---

<p class="publication-note"><sup>*</sup> Co-primary authors</p>

{% assign papers = "
pillow2025,
joey2024,
weaving2024,
spo22024,
neuro2023,
sunflower2022,
facesense2021,
teachasl2020,
threadsense2020,
<!-- polartag2020, -->
joint2019
" | split: "," %}

<div class="publication-list">
{% for raw_paper_id in papers %}
  {% assign paper_id = raw_paper_id | strip %}
  {% if paper_id != "" %}
    {% bibliography -f papers -q @*[id={{paper_id}}]* %}
  {% endif %}
{% endfor %}
</div>