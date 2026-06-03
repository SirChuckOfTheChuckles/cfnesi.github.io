---
layout: project
title: Archipelago StarCraft II Randomizer
role: Maintainer / Developer
type: Open-source game randomizer
summary: Maintainer-level work on a large open-source StarCraft II campaign randomizer, spanning gameplay logic, option systems, data files, review workflow, and difficult bug isolation.
tech:
  - Python
  - XML
  - Galaxy
  - GitHub
  - StarCraft II Editor
image: /assets/images/archipelago-sc2-banner.png
demo_url: https://archipelago.gg/
repo_url: https://github.com/ArchipelagoMW/Archipelago
order: 0
---

**Archipelago StarCraft II Randomizer** is part of the Archipelago multi-game randomizer project. It modifies StarCraft II campaign missions with randomized progression, gameplay options, mission logic, and data-driven configuration.

<div class="metric-grid">
  <div>
    <strong>80+</strong>
    <span>authored pull requests</span>
  </div>
  <div>
    <strong>75+</strong>
    <span>pull requests reviewed</span>
  </div>
  <div>
    <strong>Jul 2024</strong>
    <span>maintainer/developer start</span>
  </div>
</div>

### Impact

- Contributed 80+ pull requests across Python, XML, Galaxy scripting, and StarCraft II Editor data systems.
- Reviewed 75+ pull requests, helping maintain code quality, test bug fixes, resolve merge conflicts, and coordinate changes across forks and branches.
- Expanded option-driven gameplay logic, mission data, race-swap support, hero systems, and compatibility fixes across a large open-source codebase.
- Debugged complex generation issues caused by hidden option interactions by running repeated tests, isolating failing configurations, and tracing logic across multiple systems.
- Collaborated with maintainers and playtesters to turn bug reports, gameplay issues, and edge cases into tested implementation changes.

### Selected Contributions

<div class="contribution-list">
  <article>
    <h3>Complex Generation Debugging</h3>
    <p><strong>Problem:</strong> Certain randomized option combinations caused hard-to-reproduce generation failures.</p>
    <p><strong>Action:</strong> Reproduced failing seeds, narrowed the issue to hidden option interactions, and traced the bug through mission logic and randomized settings.</p>
    <p><strong>Result:</strong> Helped stabilize generation behavior and reduce difficult-to-diagnose failures.</p>
  </article>
  <article>
    <h3>Gameplay And Mission Compatibility</h3>
    <p><strong>Problem:</strong> New options and race-swap behavior needed to work across many mission-specific systems.</p>
    <p><strong>Action:</strong> Updated Python logic, XML data, and StarCraft II Editor systems to support mission logic, hero systems, and compatibility fixes.</p>
    <p><strong>Result:</strong> Expanded playable randomizer configurations while preserving campaign behavior across edge cases.</p>
  </article>
  <article>
    <h3>Maintainer Workflow</h3>
    <p><strong>Problem:</strong> A large open-source project needs careful review, branch coordination, and regression awareness.</p>
    <p><strong>Action:</strong> Reviewed pull requests, resolved merge conflicts, coordinated feedback, and helped convert reports from maintainers and playtesters into tested fixes.</p>
    <p><strong>Result:</strong> Supported project velocity while keeping changes reviewable and grounded in real gameplay behavior.</p>
  </article>
</div>
