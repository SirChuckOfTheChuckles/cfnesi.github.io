---
layout: default
title: Home
---

<section class="hero">
  <div class="container hero-grid">
    <div>
      <p class="eyebrow">Software Developer • Computer Science Student</p>
      <h1>Hi, I'm Charles Nesi.</h1>
      <p class="lead">
        I’m a Computer Science student at the University of Michigan focused on software development, debugging, game systems, and open-source collaboration.
      </p>
      <div class="button-row">
        <a class="button primary" href="mailto:{{ site.email }}">Contact Me</a>
        <a class="button" href="{{ site.resume_url | relative_url }}" target="_blank" rel="noopener">View Resume</a>
        <a class="button" href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener">GitHub</a>
      </div>
    </div>
    <div class="hero-card">
      <p class="hero-card-label">Currently</p>
      <h2>Seeking full-time software developer roles</h2>
      <p>
        I’m especially interested in roles where I can work on reliable software, developer tools, gameplay systems, debugging-heavy features, and collaborative engineering teams.
      </p>
    </div>
  </div>
</section>

<section id="projects" class="section">
  <div class="container">
    <div class="section-heading">
      <p class="eyebrow">Featured Work</p>
      <h2>Projects</h2>
      <p>One highlighted project to start. Add more files inside <code>_projects/</code> as the portfolio grows.</p>
    </div>

    <div class="project-grid">
      {% assign projects = site.projects | sort: 'order' %}
      {% for project in projects %}
        {% include project-card.html project=project %}
      {% endfor %}
    </div>
  </div>
</section>

<section id="experience" class="section alt">
  <div class="container two-column">
    <div>
      <p class="eyebrow">Experience</p>
      <h2>Open-source and professional work</h2>
    </div>
    <div class="timeline">
      <article>
        <h3>Archipelago Project — Maintainer / Developer</h3>
        <p class="muted">Jul 2024 – Present</p>
        <p>
          Contributed Python and XML changes to an open-source StarCraft II randomizer codebase, reviewed pull requests, resolved merge conflicts, and helped isolate complex option-driven bugs.
        </p>
      </article>
      <article>
        <h3>Quantum Services Group — Help Desk Technician</h3>
        <p class="muted">May 2025 – Aug 2025; Dec 2025</p>
        <p>
          Created and documented client support tickets, triaged hardware/software/connectivity issues, and coordinated troubleshooting with ISPs and third-party IT teams.
        </p>
      </article>
    </div>
  </div>
</section>

<section id="skills" class="section">
  <div class="container two-column">
    <div>
      <p class="eyebrow">Skills</p>
      <h2>Technical toolkit</h2>
    </div>
    <div class="skill-grid">
      <div>
        <h3>Languages</h3>
        <p>Python, C++, C#, Java, SQL, HTML/XML, Galaxy</p>
      </div>
      <div>
        <h3>Tools</h3>
        <p>Git, GitHub, Jira, Linux, Ubuntu, WSL, Unity, StarCraft II Editor</p>
      </div>
      <div>
        <h3>Strengths</h3>
        <p>Debugging, testing, documentation, troubleshooting, code organization</p>
      </div>
      <div>
        <h3>Coursework</h3>
        <p>Data Structures and Algorithms, Machine Learning, Computer Security, Web Systems, Computer Networks, Game Development</p>
      </div>
    </div>
  </div>
</section>

<section class="section cta">
  <div class="container cta-box">
    <h2>Want to get in touch?</h2>
    <p>Email is the best way to reach me for software developer opportunities.</p>
    <div class="button-row center">
      <a class="button primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
      <a class="button" href="{{ site.resume_url | relative_url }}" target="_blank" rel="noopener">Resume</a>
    </div>
  </div>
</section>
