---
layout: archive
title: ""
permalink: /team/
author_profile: false
classes: wide
---

<style>
/* =========================================================
   Ubiquitous X Lab: 
   ========================================================= */
.uxlab-hero,
.uxlab-hero * {
  box-sizing: border-box;
}

.uxlab-hero {
  --uxlab-accent: #f2ad00;
  --uxlab-text: #111111;
  --uxlab-muted: #5e5e5e;

  display: grid;
  grid-template-columns: minmax(0, 0.9fr) minmax(420px, 1.1fr);
  align-items: center;
  gap: clamp(2.5rem, 6vw, 6rem);
  width: 100%;
  max-width: 1500px;
  min-height: min(70vh, 720px);
  margin: 0 auto;
  padding: clamp(2.5rem, 6vw, 5.5rem) 0;
}

.uxlab-hero__left,
.uxlab-hero__right {
  min-width: 0;
}

.uxlab-hero__eyebrow {
  margin: 0 0 1.15rem;
  color: var(--uxlab-accent);
  font-size: clamp(0.82rem, 1vw, 1rem);
  font-weight: 800;
  letter-spacing: 0.08em;
  line-height: 1.35;
  text-transform: uppercase;
}

.uxlab-hero__title {
  margin: 0;
  padding: 0;
  border: 0;
  color: var(--uxlab-text);
  font-size: clamp(3.4rem, 5.7vw, 6.4rem);
  font-weight: 800;
  letter-spacing: -0.055em;
  line-height: 0.98;
}

.uxlab-accent {
  color: var(--uxlab-accent);
  font-weight: 750;
}

.uxlab-hero__lead {
  max-width: 39rem;
  margin: clamp(1.8rem, 3.2vw, 2.8rem) 0 0;
  color: var(--uxlab-muted);
  font-size: clamp(1.1rem, 1.6vw, 1.55rem);
  line-height: 1.68;
}

.uxlab-hero__links {
  display: flex;
  flex-wrap: wrap;
  gap: 1.1rem 2.7rem;
  margin-top: clamp(1.9rem, 3.5vw, 3rem);
}

.uxlab-hero__links a {
  color: var(--uxlab-text);
  font-size: clamp(1rem, 1.2vw, 1.18rem);
  font-weight: 800;
  text-decoration: none;
  border-bottom: 2px solid transparent;
  transition: color 160ms ease, border-color 160ms ease;
}

.uxlab-hero__links a:hover,
.uxlab-hero__links a:focus-visible {
  color: #bd8500;
  border-bottom-color: var(--uxlab-accent);
}

.uxlab-hero__media {
  position: relative;
  min-width: 0;
  overflow: hidden;
  aspect-ratio: 16 / 9;
  border: 1px solid rgba(17, 17, 17, 0.08);
  border-radius: clamp(16px, 2vw, 26px);
  background: #fff;
  box-shadow: 0 26px 65px rgba(17, 17, 17, 0.16);
}

.uxlab-hero__media img {
  display: block;
  width: 100%;
  height: 100%;
  max-width: none;
  object-fit: cover;
  object-position: center;

  /* The GIF contains generous white margins; this enlarges the logo
     while retaining the complete 16:9 animation. */
  transform: scale(1.42);
  transform-origin: center;
}

.uxlab-intro {
  max-width: 980px;
  margin: 0 auto clamp(3.5rem, 7vw, 6rem);
  padding: clamp(1.35rem, 3vw, 2.15rem) clamp(1.25rem, 3vw, 2.15rem);
  border-left: 4px solid #f2ad00;
  background: rgba(242, 173, 0, 0.075);
}

.uxlab-intro p {
  margin: 0;
  font-size: 1.04rem;
  line-height: 1.75;
}

.uxlab-intro p + p {
  margin-top: 0.9rem;
}

#our-team {
  scroll-margin-top: 6rem;
}

@media (max-width: 950px) {
  .uxlab-hero {
    grid-template-columns: 1fr;
    gap: 2.6rem;
    min-height: 0;
    padding-top: 2rem;
  }

  .uxlab-hero__left {
    max-width: 760px;
  }

  .uxlab-hero__media {
    width: 100%;
    max-width: 860px;
  }
}

@media (max-width: 600px) {
  .uxlab-hero {
    gap: 2rem;
    padding: 1.25rem 0 3rem;
  }

  .uxlab-hero__eyebrow {
    font-size: 0.75rem;
  }

  .uxlab-hero__title {
    font-size: clamp(3rem, 14vw, 4.5rem);
  }

  .uxlab-hero__lead {
    font-size: 1.05rem;
    line-height: 1.62;
  }

  .uxlab-hero__media {
    border-radius: 15px;
    box-shadow: 0 17px 40px rgba(17, 17, 17, 0.14);
  }

  .uxlab-hero__media img {
    transform: scale(1.34);
  }
}

@media (prefers-reduced-motion: reduce) {
  .uxlab-hero__links a {
    transition: none;
  }
}
</style>

<section id="home" class="uxlab-hero" aria-labelledby="uxlab-title">
  <div class="uxlab-hero__left">
    <p class="uxlab-hero__eyebrow">Exploring the Future, Enhancing Lives</p>

    <h1 id="uxlab-title" class="uxlab-hero__title">
      Ubiquitous <span class="uxlab-accent">X</span><br>Lab
    </h1>

    <p class="uxlab-hero__lead">
      We create <span class="uxlab-accent">mobile &amp; ubiquitous computing</span>
      and <span class="uxlab-accent">human-centered AI</span> systems that quietly
      transform lives in healthcare, education, and everyday interaction.
    </p>

    <nav class="uxlab-hero__links" aria-label="Lab links">
      <a href="#our-team">Our Team</a>
      <a href="{{ '/student/' | relative_url }}">Join Us</a>
    </nav>
  </div>

  <div class="uxlab-hero__right">
    <div class="uxlab-hero__media">
      <img
        src="{{ '/images/lab/logo_outside.gif' | relative_url }}"
        alt="Animated Ubiquitous X Lab logo"
        width="1280"
        height="720"
        loading="eager"
        fetchpriority="high"
        decoding="async"
      >
    </div>
  </div>
</section>

<div class="uxlab-intro">
  <p>
    At Ubiquitous X Lab, we believe technology should be both innovative and meaningful.
    Our work lives where systems, humans, and AI converge. We thrive on curiosity,
    creativity, and a shared passion for discovery.
  </p>
  <p>
    We are always looking for highly motivated postdoctoral researchers, Ph.D. students,
    and visiting scholars. Please visit our
    <strong><a href="{{ '/student/' | relative_url }}">Join Us</a></strong>
    page for current opportunities.
  </p>
</div>

<h2 id="our-team">Our Team</h2>

We are truly blessed and proud to work with an exceptional group of researchers who bring diverse expertise and enthusiasm to every project.

### Postgraduate Students
* [Jiting Liu](https://jitingliu.github.io/) (Ph.D. student, M.S. from Columbia U, Redbird Scholarship) 2025 Fall -
* [Jinhe Wen](https://jinhewen.owlstown.net/) (Ph.D. student, M.S. from UCSD) 2025 Fall -
* Yujing Zhang (Ph.D. student, M.S. from KTH) 2025 Fall -
* Yuxuan Weng (Ph.D. student, M.S. from HKUST) 2025 Fall -
* [Ziqi Liu](https://ziqidennisliu.github.io/) (M.Phil student, B.S. from Tsinghua U) 2025 Fall -

### Visiting Students/RA
* Zeyu Luo (RA, M.S. from HKUST) 2025 Spring -
* Yuchao Wang (RA, M.S. from HKUST) 2025 Spring -
* Junxiao Chen (Visiting student, Undergraduate @Tsinghua) 2025 Spring -
* Ziyi Xu (Undergraduate @HKUST) 2025 Spring -
* Jerry Yue Gong (RA, M.S. @HKUST) 2025 Spring -
* Xiangjie Tang (Visiting student, Undergraduate @Southeast) 2025 Summer -
