---
layout: default
title: Home
---

<section class="hero">
  <div class="container hero-grid">
    <div class="hero-copy">
      <p class="eyebrow">Software Developer / Computer Science Graduate</p>
      <h1>Hi, I'm Charles Nesi.</h1>
      <p class="lead">
        I build reliable software, game systems, and open-source tools with a bias toward clear debugging, readable code, and finished work.
      </p>
      <div class="button-row">
        <a class="button primary" href="#contact">Contact Me</a>
        <a class="button" href="{{ site.resume_url | relative_url }}" target="_blank" rel="noopener">View Resume</a>
        <a class="button" href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener">GitHub</a>
      </div>
      <div class="hero-proof">
        <div>
          <strong>CS</strong>
          <span>graduate with advanced technical projects</span>
        </div>
        <div>
          <strong>Broad Toolkit</strong>
          <span>Python, C++, C#, Java, SQL, XML, and Galaxy</span>
        </div>
        <div>
          <strong>2</strong>
          <span>featured shipped projects</span>
        </div>
      </div>
    </div>

    <div class="hero-visual" aria-label="Snapshot of Charles Nesi's software work">
      <div class="code-window">
        <div class="window-bar">
          <span></span>
          <span></span>
          <span></span>
        </div>
        <pre><code>class Developer:
    focus = [
        "debugging",
        "game systems",
        "open source",
        "tools"
    ]

    def ship(self, project):
        test(project)
        document(project)
        return "ready"</code></pre>
      </div>
      <div class="status-card">
        <strong>Seeking full-time software developer roles</strong>
        <span>Specialized in reliable tools, gameplay systems, debugging, and maintainable engineering work.</span>
      </div>
    </div>
  </div>
</section>

<section class="intro-band">
  <div class="container intro-grid">
    <p>
      I am a Computer Science graduate who completed my CS coursework at the University of Michigan. I enjoy projects where the hard part is understanding the system: tracing behavior, fixing edge cases, and optimizing existing systems so they can support greater capabilities.
    </p>
  </div>
</section>

<section id="projects" class="section">
  <div class="container">
    <div class="section-heading">
      <p class="eyebrow">Featured Work</p>
      <h2>Projects</h2>
      <p>Some of my work that shows shipped projects, collaboration, and practical engineering judgment.</p>
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
      <h2>Open-Source and Professional Work</h2>
    </div>
    <div class="timeline">
      <article>
        <h3>Archipelago Project - Maintainer / Developer</h3>
        <p class="muted">Jul 2024 - Present</p>
        <p>
          Contributed 80+ pull requests and reviewed 75+ more for an open-source StarCraft II randomizer, working across Python, XML, Galaxy scripting, StarCraft II Editor data, and option-driven gameplay systems.
        </p>
      </article>
      <article>
        <h3>Quantum Services Group - Help Desk Technician</h3>
        <p class="muted">May 2025 - Aug 2025; Dec 2025</p>
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
      <h2>Technical Toolkit</h2>
    </div>
    <div class="skill-grid">
      <div>
        <h3>Languages</h3>
        <p>Python, C++, C#, Java, SQL, HTML/XML, Galaxy</p>
      </div>
      <div>
        <h3>Tools</h3>
        <p>Git, GitHub, Jira, Linux, Ubuntu, WSL, Unity, SC II Editor</p>
      </div>
      <div>
        <h3>Strengths</h3>
        <p>Debugging, optimization, documentation, simplification, code organization</p>
      </div>
      <div>
        <h3>Coursework</h3>
        <p>Data Structures and Algorithms, Machine Learning, Computer Security, Web Systems, Computer Networks, Game Development</p>
      </div>
    </div>
  </div>
</section>

<section id="contact" class="section cta">
  <div class="container cta-box">
    <h2>Contact</h2>
    <div class="contact-list">
      <a class="contact-item" href="mailto:{{ site.email }}">
        <span>Email</span>
        <strong>{{ site.email }}</strong>
      </a>
      {% if site.phone != blank %}
        <a class="contact-item" href="tel:{{ site.phone | remove: ' ' | remove: '-' | remove: '(' | remove: ')' | remove: '.' }}">
          <span>Phone</span>
          <strong>{{ site.phone }}</strong>
        </a>
      {% endif %}
    </div>
  </div>
</section>
