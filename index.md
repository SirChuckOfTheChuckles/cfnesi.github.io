---
layout: default
title: Home
---

<section class="hero">
  <div class="container hero-grid">
    <div class="hero-copy">
      <p class="eyebrow">Software Developer / Computer Science Student</p>
      <h1>Hi, I'm Charles Nesi.</h1>
      <p class="lead">
        I build reliable software, game systems, and open-source tools with a bias toward clear debugging, readable code, and finished work.
      </p>
      <div class="button-row">
        <a class="button primary" href="mailto:{{ site.email }}">Contact Me</a>
        <a class="button" href="{{ site.resume_url | relative_url }}" target="_blank" rel="noopener">View Resume</a>
        <a class="button" href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener">GitHub</a>
      </div>
      <div class="hero-proof">
        <div>
          <strong>80+</strong>
          <span>open-source PRs authored</span>
        </div>
        <div>
          <strong>75+</strong>
          <span>pull requests reviewed</span>
        </div>
        <div>
          <strong>1</strong>
          <span>released game project</span>
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
      <div class="status-strip">
        <span>Currently seeking full-time software roles</span>
        <span>Northville, MI</span>
      </div>
    </div>
  </div>
</section>

<section class="intro-band">
  <div class="container intro-grid">
    <p>
      I am a Computer Science student at the University of Michigan who likes projects where the hard part is understanding the system: tracing behavior, fixing edge cases, and making the result easier for the next person to work with.
    </p>
    <a href="#projects">Explore featured work</a>
  </div>
</section>

<section id="projects" class="section">
  <div class="container">
    <div class="section-heading">
      <p class="eyebrow">Featured Work</p>
      <h2>Projects</h2>
      <p>Selected work that shows shipped projects, collaboration, and practical engineering judgment.</p>
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
      <h2>Open-source and professional work.</h2>
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
      <h2>Technical toolkit.</h2>
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
