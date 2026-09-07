---
layout: archive
title: ""
permalink: /team/
author_profile: false
classes: wide
---

<style>

  /* =========================================================
   GLOBAL LAB COLORS
   ========================================================= */

:root {
  --uxlab-accent: #f2ad00;
  --uxlab-text: #111111;
  --uxlab-muted: #5e5e5e;
}


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
  grid-template-columns: minmax(0, 1.2fr) minmax(360px, 0.8fr);
  align-items: center;

  gap: clamp(1rem, 2.5vw, 3rem);

  width: 100%;
  max-width: 1450px;
  min-height:auto;

  margin: -1rem auto 0;
  padding: 0;
}


/* =========================================================
   LEFT COLUMN
   ========================================================= */

.uxlab-hero__left,
.uxlab-hero__right {
  min-width: 0;
}

.uxlab-hero__right {
  display: flex;
  flex-direction: column;
  align-items: stretch;

  width: 100%;

  justify-self: end;
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
  max-width: 48rem;

  margin: 1rem 0 0;

  color: var(--uxlab-muted);

  font-size: clamp(1rem, 1.25vw, 1.3rem);
  line-height: 1.65;

  /* text-align: justify;
  text-justify: inter-word; */
}


/* Hero links */
.uxlab-hero__links {
  display: flex;
  flex-wrap: wrap;

  gap: 1rem 2.4rem;

  margin-top: 1rem;
}

.uxlab-hero__links--right {
  justify-content: flex-end;

  width: 100%;

  gap: 1.5rem;

  margin-top: 1.4rem;
}


.uxlab-hero__links a {
  color: var(--uxlab-text);

  font-size: clamp(0.95rem, 1.05vw, 1.1rem);
  font-weight: 800;

  text-decoration: none !important;
  border-bottom: 2px solid transparent;

  transition:
    color 160ms ease,
    border-color 160ms ease;
}

.uxlab-hero__links a:hover,
.uxlab-hero__links a:focus,
.uxlab-hero__links a:focus-visible,
.uxlab-hero__links a:active {
  color: var(--uxlab-accent) !important;

  text-decoration: none !important;

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
   TEAM SECTION
   ========================================================= */

.uxlab-team-section {
  margin-top: 0;
}

/* All normal links in the team section use the lab accent */
.uxlab-team-section a,
.uxlab-team-section a:visited {
  color: var(--uxlab-accent) !important;
  text-decoration: none !important;
}

.uxlab-team-section a:hover,
.uxlab-team-section a:focus,
.uxlab-team-section a:focus-visible {
  color: var(--uxlab-accent) !important;
  text-decoration: underline !important;
  text-decoration-color: var(--uxlab-accent) !important;
  text-underline-offset: 0.12em;
}


/* =========================================================
   POSTGRADUATE STUDENT GRID
   ========================================================= */

.uxlab-student-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 1.6rem;
  margin-top: 1.5rem;
  margin-bottom: 3.5rem;
}

.uxlab-student-card {
  min-width: 0;
  text-align: center;
}

.uxlab-student-photo {
  width: 100%;
  aspect-ratio: 1 / 1;
  overflow: hidden;
  border-radius: 14px;
  background: #f3f3f3;
}

.uxlab-student-photo img {
  display: block;
  width: 100%;
  height: 100%;
  max-width: none;
  object-fit: cover;
  object-position: center;
  transition: transform 180ms ease;
}

.uxlab-student-card a:hover .uxlab-student-photo img {
  transform: scale(1.025);
}

.uxlab-student-name {
  margin-top: 0.9rem;
  margin-bottom: 0.22rem;
  font-size: 1.12rem;
  font-weight: 800;
  line-height: 1.3;
}

.uxlab-student-name a {
  color: #111111;
  text-decoration: none !important;
}

.uxlab-student-name a:hover,
.uxlab-student-name a:focus-visible {
  color: #bd8500;
  text-decoration: none !important;
}

.uxlab-student-info {
  margin: 0;
  color: #666666;
  font-size: 0.9rem;
  line-height: 1.5;
}

@media (max-width: 1000px) {
  .uxlab-student-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }
}

@media (max-width: 750px) {
  .uxlab-student-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 520px) {
  .uxlab-student-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
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
      At Ubiquitous X Lab, we believe technology should be both innovative and meaningful. 
      We create

      <span class="uxlab-accent">
        mobile &amp; ubiquitous computing
      </span>

      and

      <span class="uxlab-accent">
        human-centered AI systems
      </span>

      that quietly transform lives in
      healthcare, education, and everyday interaction.

    </p>



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
  
  <nav
      class="uxlab-hero__links uxlab-hero__links--right"
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

</section>





## Our Team
We are truly blessed and proud to work with an exceptional group of researchers who bring diverse expertise and enthusiasm to every project.


<div class="lab-photo-carousel" aria-label="Ubiquitous X Lab photos">

  <div class="lab-photo-slide is-active">
    <img src="{{ '/images/lab/lab-group-1.jpg' | relative_url }}"
         alt="Ubiquitous X Lab group photo">
  </div>

  <div class="lab-photo-slide">
    <img src="{{ '/images/lab/lab-group-2.jpg' | relative_url }}"
         alt="Ubiquitous X Lab activity">
  </div>

  <div class="lab-photo-slide">
    <img src="{{ '/images/lab/lab-group-3.jpg' | relative_url }}"
         alt="Ubiquitous X Lab group event">
  </div>

  <div class="lab-photo-slide">
    <img src="{{ '/images/lab/lab-group-4.jpg' | relative_url }}"
         alt="Ubiquitous X Lab presentation">
  </div>

</div>

### Faculty
<div class="uxlab-student-grid">

  <div class="uxlab-student-card">
    <a href="https://qijiashao.github.io/" target="_blank" rel="noopener noreferrer">
      <div class="uxlab-student-photo">
        <img src="{{ '/images/lab/people/qijia-shao.jpg' | relative_url }}" alt="Qijia Shao">
      </div>
    </a>
    <div class="uxlab-student-name">
      <a href="qijiashao.github.io/" target="_blank" rel="noopener noreferrer">Qijia Shao</a>
    </div>
    <p class="uxlab-student-info">
      PI / Assistant Professor
    </p>
  </div>
</div>

### Postgraduate Students

<div class="uxlab-student-grid">

  <div class="uxlab-student-card">
    <a href="https://jitingliu.github.io/" target="_blank" rel="noopener noreferrer">
      <div class="uxlab-student-photo">
        <img src="{{ '/images/lab/people/jiting-liu.jpg' | relative_url }}" alt="Jiting Liu">
      </div>
    </a>
    <div class="uxlab-student-name">
      <a href="https://jitingliu.github.io/" target="_blank" rel="noopener noreferrer">Jiting Liu</a>
    </div>
    <p class="uxlab-student-info">
      Ph.D. Student<br>
      M.S. from Columbia University<br>
      Redbird Scholarship<br>
      2025 Fall –
    </p>
  </div>

  <div class="uxlab-student-card">
    <a href="https://jinhewen.owlstown.net/" target="_blank" rel="noopener noreferrer">
      <div class="uxlab-student-photo">
        <img src="{{ '/images/lab/people/jinhe-wen.jpg' | relative_url }}" alt="Jinhe Wen">
      </div>
    </a>
    <div class="uxlab-student-name">
      <a href="https://jinhewen.owlstown.net/" target="_blank" rel="noopener noreferrer">Jinhe Wen</a>
    </div>
    <p class="uxlab-student-info">
      Ph.D. Student<br>
      M.S. from UCSD<br>
      2025 Fall –
    </p>
  </div>

  <div class="uxlab-student-card">
    <div class="uxlab-student-photo">
      <img src="{{ '/images/lab/people/yujing-zhang.jpg' | relative_url }}" alt="Yujing Zhang">
    </div>
    <div class="uxlab-student-name">Yujing Zhang</div>
    <p class="uxlab-student-info">
      Ph.D. Student<br>
      M.S. from KTH<br>
      2025 Fall –
    </p>
  </div>

  <div class="uxlab-student-card">
    <div class="uxlab-student-photo">
      <img src="{{ '/images/lab/people/yuxuan-weng.jpg' | relative_url }}" alt="Yuxuan Weng">
    </div>
    <div class="uxlab-student-name">Yuxuan Weng</div>
    <p class="uxlab-student-info">
      Ph.D. Student<br>
      M.S. from HKUST<br>
      2025 Fall –
    </p>
  </div>

  <div class="uxlab-student-card">
    <a href="https://ziqidennisliu.github.io/" target="_blank" rel="noopener noreferrer">
      <div class="uxlab-student-photo">
        <img src="{{ '/images/lab/people/ziqi-liu.jpg' | relative_url }}" alt="Ziqi Liu">
      </div>
    </a>
    <div class="uxlab-student-name">
      <a href="https://ziqidennisliu.github.io/" target="_blank" rel="noopener noreferrer">Ziqi Liu</a>
    </div>
    <p class="uxlab-student-info">
      M.Phil Student<br>
      B.S. from Tsinghua University<br>
      2025 Fall –
    </p>
  </div>

  <div class="uxlab-student-card">
    <div class="uxlab-student-photo">
      <img src="{{ '/images/lab/people/junxiao-chen.jpg' | relative_url }}" alt="Junxiao Chen">
    </div>
    <div class="uxlab-student-name">Junxiao Chen</div>
    <p class="uxlab-student-info">
      Ph.D. Student<br>
      B.S. from Tsinghua University<br>
      2026 Fall –
    </p>
  </div>

</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const slides = document.querySelectorAll(".lab-photo-slide");

  if (slides.length <= 1) return;

  let current = 0;

  setInterval(function () {
    slides[current].classList.remove("is-active");

    current = (current + 1) % slides.length;

    slides[current].classList.add("is-active");
  }, 4000);
});
</script>

### Visiting Students/RA
* [Zeyu Luo]() (RA, M.S. from HKUST) 2025 Spring - 
* [Jerry Yue Gong]() (RA, M.S. @HKUST) 2025 Spring - 
* [Xuye You]() (Undergraduate @HKUST) 2026 Summer - 
* [Madi Liang]() (RA, M.S. from Queensland) 2026 Summer - 
* [Sibo Wang]() (Visiting Student, M.S. @Tongji) 2026 Summer - 


### Alumni
* [Junxiao Chen]() Undergraduate (2025-2026)  Now Ph.D. student at HKUST.
* [Xiangjie Tang]() Visiting Student (2025-2026), Now Ph.D. student at Seoul National University.
* [Ziyi Xu]() Undergraduate (2025-2026), Now Ph.D. student at HKUST.
* [Yuchao Wang]() RA (2025-2026), Now M.Phil student at HKUST.

