---
layout: home
title: Home
---

<section class="hero">
  <div class="hero__content">
    <p class="hero__eyebrow">Carnegie Mellon University · Electrical &amp; Computer Engineering · Class of 2029</p>
    <h1 class="hero__title">Hi, I'm Zhaojin Chu.</h1>
    <p class="hero__lead">
      I design machine learning systems, full-stack products, and learning experiences that help people understand and use
      technology with confidence. I split my time between research labs, hardware benches, and classrooms where I teach the next
      wave of engineers.
    </p>
    <div class="hero__buttons">
      <a class="button button--primary" href="{{ '/cv' | relative_url }}">View résumé</a>
      <a class="button button--ghost" href="mailto:{{ site.author.email }}">Start a conversation</a>
    </div>
    <ul class="hero__details">
      <li>Founder of Logic Labs, delivering hands-on electronics kits and workshops to 60+ students across the Gulf.</li>
      <li>Currently building license plate perception systems and music scheduling tools that serve real communities.</li>
      <li>Based in Pittsburgh, PA and Dubai, UAE — open to collaborations and 2026 engineering internships.</li>
    </ul>
  </div>
  <div class="hero__media">
    <img class="hero__portrait" src="{{ site.photo | relative_url }}" alt="Portrait of Zhaojin Chu">
  </div>
</section>

<section class="section" id="snapshot">
  <div class="section__heading">
    <h2 class="section-title">Snapshot</h2>
    <p class="section-subtitle">Where my energy is going right now.</p>
  </div>
  <div class="stat-grid">
    <article class="stat-card">
      <h3>Building thoughtful systems</h3>
      <p>
        From real-time license plate recognition to survey analytics on generative AI, I prototype end-to-end solutions and push
        them into the hands of people who need them. I love pairing rigorous models with lightweight deployment strategies.
      </p>
    </article>
    <article class="stat-card">
      <h3>Technical toolkit</h3>
      <ul>
        <li>Languages: Python, C, JavaScript/TypeScript, SQL, HTML/CSS, LaTeX</li>
        <li>Frameworks: PyTorch, Django, React, Celery, Tailwind</li>
        <li>Hardware &amp; tools: KiCad, Fusion 360, ONNX Runtime, Stripe APIs, Git</li>
      </ul>
    </article>
    <article class="stat-card">
      <h3>What I'm exploring next</h3>
      <p>
        Scaling Logic Labs' kit library, compressing neural networks for edge inference, and blending AI literacy with music
        education. Always eager to co-create with teams that care about impact and craft.
      </p>
    </article>
  </div>
</section>

<section class="section" id="experience">
  <div class="section__heading">
    <h2 class="section-title">Experience</h2>
    <p class="section-subtitle">Leading teams and shipping tools that make technology approachable.</p>
  </div>
  <div class="timeline">
    <article class="timeline__item">
      <span class="timeline__badge" aria-hidden="true"></span>
      <h3 class="timeline__title">Logic Labs &middot; Founder &amp; Lead Developer</h3>
      <p class="timeline__meta">Jan 2024 – Present · Dubai &amp; Pittsburgh</p>
      <div class="timeline__body">
        <ul>
          <li>Delivered curated electronics kits and lectures to 60+ middle and high school students, designing each cohort's lab roadmap.</li>
          <li>Built a Node.js/React e-commerce platform with Stripe billing, logistics workflows, and educator dashboards for curriculum planning.</li>
          <li>Coach a volunteer developer team, synthesize student feedback, and expand the hardware lineup for upcoming cohorts.</li>
        </ul>
      </div>
    </article>
    <article class="timeline__item">
      <span class="timeline__badge" aria-hidden="true"></span>
      <h3 class="timeline__title">Cobblestone Energy &middot; Data Analyst / IT Intern</h3>
      <p class="timeline__meta">Dec 2023 · Dubai</p>
      <div class="timeline__body">
        <ul>
          <li>Engineered a UK-wide, weather-aware day-ahead forecasting pipeline using lag features, rolling statistics, and walk-forward validation.</li>
          <li>Partnered with traders to stress-test inference latency and turn model insights into actionable energy procurement strategies.</li>
        </ul>
      </div>
    </article>
  </div>
</section>

<section class="section" id="projects">
  <div class="section__heading">
    <h2 class="section-title">Selected Projects</h2>
    <p class="section-subtitle">A rotating sample of the research, products, and experiments I'm documenting.</p>
  </div>
  <ul class="project-list">
    {% assign featured_projects = site.projects | sort: 'order' %}
    {% for project in featured_projects limit: 3 %}
    <li class="project-card">
      {% if project.category %}<span class="project-card__label">{{ project.category }}</span>{% endif %}
      <a class="project-card__title" href="{{ project.url | relative_url }}">{{ project.title }}</a>
      <p class="project-card__summary">{{ project.summary }}</p>
      <ul class="project-card__meta">
        {% if project.timeline %}<li>{{ project.timeline }}</li>{% endif %}
        {% if project.skills %}<li>{{ project.skills | join: ' · ' }}</li>{% endif %}
      </ul>
    </li>
    {% endfor %}
  </ul>
  <a class="arrow-link" href="{{ '/projects' | relative_url }}">Browse the full project journal</a>
</section>

<section class="section" id="leadership">
  <div class="section__heading">
    <h2 class="section-title">Leadership &amp; Community</h2>
    <p class="section-subtitle">Teaching, organizing, and performing to keep curiosity alive.</p>
  </div>
  <div class="stat-grid">
    <article class="stat-card">
      <h3>Top University Prep Program</h3>
      <p>
        Designed STEM intensives and mentoring pathways for 100+ high school students aiming for global universities. Built project-based
        modules, coached interview prep, and coordinated guest speakers across time zones.
      </p>
    </article>
    <article class="stat-card">
      <h3>National Youth Orchestra of Dubai &amp; Viola Club</h3>
      <p>
        First chair violist and club president, curating performance repertoires and arranging community concerts that blend classical
        technique with regional music traditions.
      </p>
    </article>
    <article class="stat-card">
      <h3>Community Stewardship</h3>
      <p>
        Led Dubai College's Computer Hardware Society, volunteered at The Old Library, and completed the Duke of Edinburgh Gold Award with a
        focus on service and outdoor leadership.
      </p>
    </article>
  </div>
</section>

<section class="section" id="honors">
  <div class="section__heading">
    <h2 class="section-title">Honors &amp; Awards</h2>
    <p class="section-subtitle">Celebrating teams, mentors, and opportunities that shaped my path.</p>
  </div>
  <ul class="badge-grid">
    <li class="badge">Netcraft Computer Science Prize Top 100 Global · 2025</li>
    <li class="badge">Computer Science Award · 2025</li>
    <li class="badge">Duke of Edinburgh Gold Award · 2025</li>
    <li class="badge">Mathematical Challenge Gold Award · 2023</li>
    <li class="badge">Pearson High Achiever Award · 2023</li>
    <li class="badge">Associate of the Royal Schools of Music Diploma · 2022</li>
  </ul>
</section>

<section class="section" id="contact">
  {% include contact.html %}
</section>
