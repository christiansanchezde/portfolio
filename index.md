---
layout: default
---

## About Me
Innovation isn’t just about the "new", it’s about understanding the "why." My background as a researcher taught me how to ask the right questions; my career as a software engineer taught me how to build the right answers. I have a particular affinity for hardware-level challenges and, perhaps unusually, a deep respect for legacy code. I see old systems as a masterclass in engineering logic—lessons that allow me to build more resilient solutions for the future. I thrive in teams where communication is a tool, not an afterthought, and where trust is the foundation of every sprint.

## Technical Skills
### Software
<div class="skill-tags">
    <span class="skill-tag">Python</span>
    <span class="skill-tag">C++17</span>
    <span class="skill-tag">Rust</span>
    <span class="skill-tag">PyTorch</span>
    <span class="skill-tag">CUDA</span>
    <span class="skill-tag">Docker</span>
    <span class="skill-tag">Kubernetes</span>
    <span class="skill-tag">AWS</span>
</div>

### others
<div class="skill-tags">
    <span class="skill-tag">Python</span>
    <span class="skill-tag">C++17</span>
    <span class="skill-tag">Rust</span>
    <span class="skill-tag">PyTorch</span>
    <span class="skill-tag">CUDA</span>
    <span class="skill-tag">Docker</span>
    <span class="skill-tag">Kubernetes</span>
    <span class="skill-tag">AWS</span>
</div>

## Selected Publications & Thesis
{% for pub in site.data.publications %}
<div class="pub-item">
    <a href="{{ pub.url }}" class="pub-title" target="_blank">{{ pub.title }}</a>
    <span class="pub-meta">
        {{ pub.type }} | {{ pub.context }}, {{ pub.year }}
    </span>
</div>
{% endfor %}

## Personal Projects
<div class="project-grid">
{% for project in site.data.projects %}
    <div class="project-card">
        <h3>{{ project.name }}</h3>
        <p>{{ project.description }}</p>
        <div class="skill-tags" style="margin-bottom: 0.8rem;">
            {% for tag in project.tags %}
            <span class="skill-tag" style="background: #21262d;">{{ tag }}</span>
            {% endfor %}
        </div>
        <a href="{{ project.url }}" class="project-link" target="_blank">View on GitHub &rarr;</a>
    </div>
{% endfor %}
</div>