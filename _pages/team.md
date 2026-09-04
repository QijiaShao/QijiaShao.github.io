---
layout: archive
title: ""
permalink: /team/
author_profile: false
classes: wide
---

<style>
/* =========================================================
   Ubiquitous X Lab Hero
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

  gap: clamp(2.5rem, 5vw, 5rem);

  width: 100%;
  max-width: 1450px;
  min-height: min(68vh, 700px);

  margin: 0 auto;
  padding: clamp(2.5rem, 5vw, 5rem) 0;
}


/* =========================================================
   LEFT COLUMN
   ========================================================= */

.uxlab-hero__left,
.uxlab-hero__right {
  min-width: 0;
}


/* Small orange slogan */
.uxlab-hero__eyebrow {
  margin: 0 0 1.2rem;

  color: var(--uxlab-accent);

  font-size: clamp(0.72rem, 0.9vw, 0.9rem);
  font-weight: 800;

  letter-spacing: 0.06em;
  line-height: 1.35;

  text-transform: uppercase;
}


/* Main title */
.uxlab-hero__title {
  margin: 0;
  padding: 0;
  border: 0;

  color: var(--uxlab-text);

  font-size: clamp(2.1rem, 3vw, 3.6rem);
  font-weight: 800;

  letter-spacing: -0.035em;
  line-height: 1.02;
}


/* Force "Lab" onto second line */
.uxlab-title-line {
  display: block;
}


/* Orange X and highlighted phrases */
.uxlab-accent {
  color: var(--uxlab-accent);
  font-weight: 750;
}


/* Main description */
.uxlab-hero__lead {
  max-width: 40rem;

  margin: 2rem 0 0;

  color: var(--uxlab-muted);

  font-size: clamp(1rem, 1.25vw, 1.3rem);
  line-height: 1.65;
}


/* Hero links */
.uxlab-hero__links {
  display: flex;
  flex-wrap: wrap;

  gap: 1rem 2.4rem;

  margin-top: 2.2rem;
}


.uxlab-hero__links a {
  color: var(--uxlab-text);

  font-size: clamp(0.95rem, 1.05vw, 1.1rem);
  font-weight: 800;

  text-decoration: none;

  border-bottom: 2px solid transparent;

  transition:
    color 160ms ease,
    border-color 160ms ease;
}


.uxlab-hero__links a:hover,
.uxlab-hero__links a:focus-visible {
  color: #bd8500;
  border-bottom-color: var(--uxlab-accent);
}


/* =========================================================
   RIGHT COLUMN: ANIMATED LOGO
   ========================================================= */

.uxlab-hero__media {
  position: relative;

  min-width: 0;

  overflow: hidden;

  aspect-ratio: 16 / 9;

  border: 1px solid rgba(17, 17, 17, 0.08);
  border-radius: clamp(16px, 2vw, 26px);

  background: #ffffff;

  box-shadow:
    0 25px 60px rgba(17, 17, 17, 0.15);
}


.uxlab-hero__media img {
  display: block;

  width: 100%;
  height: 100%;

  max-width: none;

  object-fit: cover;
  object-position: center;

  /*
     The GIF has considerable whitespace.
     Increase/decrease this number if needed.
  */
  transform: scale(1.45);
  transform-origin: center;
}


/* =========================================================
   INTRODUCTION BOX BELOW HERO
   ========================================================= */

.uxlab-intro {
  max-width: 980px;

  margin:
    0 auto
    clamp(3.5rem, 7vw, 6rem);

  padding:
    clamp(1.3rem, 3vw, 2rem)
    clamp(1.3rem, 3vw, 2rem);

  border-left: 4px solid #f2ad00;

  background: rgba(242, 173, 0, 0.07);
}


.uxlab-intro p {
  margin: 0;

  font-size: 1.04rem;
  line-height: 1.75;
}


.uxlab-intro p + p {
  margin-top: 0.9rem;
}


/* Give anchor links some space below top navigation */
#our-team {
  scroll-margin-top: 6rem;
}


/* =========================================================
   TABLET
   ========================================================= */

@media (max-width: 950px) {

  .uxlab-hero {
    grid-template-columns: 1fr;

    gap: 2.8rem;

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


  .uxlab-hero__title {
    font-size: clamp(2.7rem, 7vw, 4.4rem);
  }


  .uxlab-hero__lead {
    max-width: 44rem;
  }
}


/* =========================================================
   MOBILE
   ========================================================= */

@media (max-width: 600px) {

  .uxlab-hero {
    gap: 2rem;

    padding:
      1.3rem 0
      3rem;
  }


  .uxlab-hero__eyebrow {
    margin-bottom: 0.9rem;

    font-size: 0.72rem;
  }


  .uxlab-hero__title {
    font-size: clamp(2.7rem, 13vw, 4rem);

    letter-spacing: -0.03em;

    line-height: 1;
  }


  .uxlab-hero__lead {
    margin-top: 1.6rem;

    font-size: 1rem;
    line-height: 1.6;
  }


  .uxlab-hero__links {
    margin-top: 1.7rem;
  }


  .uxlab-hero__media {
    border-radius: 15px;

    box-shadow:
      0 17px 40px rgba(17, 17, 17, 0.13);
  }


  .uxlab-hero__media img {
    transform: scale(1.34);
  }


  .uxlab-intro {
    margin-bottom: 3.5rem;
  }
}


/* =========================================================
   ACCESSIBILITY
   ========================================================= */

@media (prefers-reduced-motion: reduce) {

  .uxlab-hero__links a {
    transition: none;
  }

}
</style>


<section
  id="home"
  class="uxlab-hero"
  aria-labelledby="uxlab-title"
>

  <div class="uxlab-hero__left">

    <p class="uxlab-hero__eyebrow">
      Exploring the Future, Enhancing Lives
    </p>


    <h1 id="uxlab-title" class="uxlab-hero__title">
    Ubiquitous <span class="uxlab-accent">X</span> Lab
    </h1>


    <p class="uxlab-hero__lead">

      We create

      <span class="uxlab-accent">
        mobile &amp; ubiquitous computing
      </span>

      and

      <span class="uxlab-accent">
        human-centered AI
      </span>

      systems that quietly transform lives in
      healthcare, education, and everyday interaction.

    </p>


    <nav
      class="uxlab-hero__links"
      aria-label="Lab links"
    >

      <a
        href="https://www.youtube.com/@UbiquitousX-HKUST"
        target="_blank"
        rel="noopener noreferrer"
      >
        YouTube
      </a>

      <a href="{{ '/student/' | relative_url }}">
        Join Us
      </a>

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
    At Ubiquitous X Lab, we believe technology should be both
    innovative and meaningful. Our work lives where systems, humans,
    and AI converge. We are driven by a deep purpose — using mobile
    and ubiquitous computing to quietly transform lives, especially
    in healthcare, education, and interaction.
  </p>

  <p>
    We thrive on curiosity, creativity, and a shared passion for
    discovery. We are always looking for highly motivated
    postdoctoral researchers, Ph.D. students, and visiting scholars.
    Please visit our
    <strong>
      <a href="{{ '/student/' | relative_url }}">
        Join Us
      </a>
    </strong>
    page for current opportunities.
  </p>

</div>



## Our Team
We are truly blessed and proud to work with an exceptional group of researchers who bring diverse expertise and enthusiasm to every project.

### Postgraduate Students
* [Jiting Liu](https://jitingliu.github.io/) (Ph.D. student, M.S. from Columbia U, Redbird Scholarship) 2025 Fall -
* [Jinhe Wen](https://jinhewen.owlstown.net/) (Ph.D. student, M.S. from UCSD) 2025 Fall -
* [Yujing Zhang]() (Ph.D. student, M.S. from KTH) 2025 Fall -
* [Yuxuan Weng]() (Ph.D. student, M.S. from HKUST) 2025 Fall - 
* [Ziqi Liu](https://ziqidennisliu.github.io/) (M.Phil student, B.S. from Tsinghua U) 2025 Fall - 
* [Junxiao Chen]() (Ph.D. student, B.S. from Tsinghua U) 2026 Fall - 

### Visiting Students/RA
* [Zeyu Luo]() (RA, M.S. from HKUST) 2025 Spring - 
* [Jerry Yue Gong]() (RA, M.S. @HKUST) 2025 Spring - 


### Alumni
* [Junxiao Chen]() Undergraduate (2025-2026)  Now Ph.D. student at HKUST.
* [Xiangjie Tang]() Visiting Student (2025-2026), Now Ph.D. student at Seoul National University.
* [Ziyi Xu]() Undergraduate (2025-2026), Now Ph.D. student at HKUST.
* [Yuchao Wang]() RA (2025-2026), Now M.Phil student at HKUST.