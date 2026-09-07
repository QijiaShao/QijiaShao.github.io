---
layout: single
permalink: /
title: "About Me"
excerpt: "Practically deployable new sensing rationale and generalizable AI systems for understanding human behavior and physiology."
author_profile: true
show_affiliation_logo: false
home_news_limit: 8
redirect_from:
  - /about/
  - /about.html
---

<div class="home-page">

  <p class="home-lead">
    I am an Assistant Professor at the
    <a href="https://hkust.edu.hk/">Hong Kong University of Science and Technology (HKUST)</a>.
    Our lab creates <strong>practically deployable sensing rationale and generalizable AI systems</strong>
    to understand human behavior and physiology, with applications in healthcare,
    education, and interaction.
  </p>

  <aside class="home-callout" aria-labelledby="home-openings-title">
    <h2 id="home-openings-title">Join our group</h2>
    <p>
      We have openings for postdoctoral researchers, Ph.D. students, and visiting students.
      Prospective Ph.D. applicants are encouraged to undertake an internship with us before applying.
    </p>
    <a class="home-cta" href="{{ '/student/' | relative_url }}">
      Explore opportunities <span aria-hidden="true">&rarr;</span>
    </a>
  </aside>

  <section class="home-section" aria-labelledby="home-research-title">
    <h2 id="home-research-title">Research</h2>
    <p>
      We combine physical and physiological sensing with hardware–software co-design
      to understand human states and address real-world challenges.
      Our work focuses on two complementary directions.
    </p>

    <div class="home-research-grid">
      <div class="home-research-card">
        <h3>Hardware &amp; System Design</h3>
        <p>
          Build unobtrusive systems that capture useful human signals while preserving
          a natural, comfortable user experience.
        </p>
      </div>

      <div class="home-research-card">
        <h3>Software &amp; Algorithms</h3>
        <p>
          Develop computationally efficient algorithms that work with limited data
          and generalize to new users and environments.
        </p>
      </div>
    </div>

    <nav class="home-links" aria-label="Explore our research">
      <a href="{{ '/team/' | relative_url }}">Ubiquitous X Lab <span aria-hidden="true">&rarr;</span></a>
      <a href="{{ '/publications/' | relative_url }}">Selected publications <span aria-hidden="true">&rarr;</span></a>
    </nav>
  </section>

  <section class="home-section" aria-labelledby="home-background-title">
    <h2 id="home-background-title">Background</h2>
    <p>
      I received my Ph.D. in Computer Science from
      <a href="https://www.columbia.edu/">Columbia University</a> in 2024,
      advised by <a href="https://www.cs.columbia.edu/~xia/">Xia Zhou</a> and
      <a href="http://fredjiang.com/">Fred Jiang</a>.
      Before that, I earned my master's degree from
      <a href="https://home.dartmouth.edu/">Dartmouth College</a> and my bachelor's degree from
      <a href="https://en.uestc.edu.cn/">UESTC</a>.
    </p>
  </section>

  {% assign home_news = site.data.home_news %}
  {% assign news_limit = page.home_news_limit | default: 5 %}

  {% if home_news and home_news.size > 0 %}
  <section class="home-section" aria-labelledby="home-news-title">
    <h2 id="home-news-title">Recent News</h2>

    <ul class="home-news-list" role="list">
      {% for item in home_news limit: news_limit %}
      <li class="home-news-item">
        <time class="home-news-date" datetime="{{ item.date | split: '/' | last }}-{{ item.date | split: '/' | first }}">{{ item.date }}</time>
        <div class="home-news-text">{{ item.text | markdownify }}</div>
      </li>
      {% endfor %}
    </ul>

    {% if home_news.size > news_limit %}
    <details class="home-news-archive">
      <summary>Earlier news</summary>

      <ul class="home-news-list" role="list">
        {% for item in home_news offset: news_limit %}
        <li class="home-news-item">
          <time class="home-news-date" datetime="{{ item.date | split: '/' | last }}-{{ item.date | split: '/' | first }}">{{ item.date }}</time>
          <div class="home-news-text">{{ item.text | markdownify }}</div>
        </li>
        {% endfor %}
      </ul>
    </details>
    {% endif %}
  </section>
  {% endif %}

</div>