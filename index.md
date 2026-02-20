---
layout: default
---

## About Me
I’ve always believed that real innovation starts with understanding the "why" behind a system. My background in research taught me how to ask the right questions, while my experience as an engineer taught me how to build practical, reliable answers.

I have a particular affinity for hardware-level challenges and a deep respect for legacy code. I see older systems as a masterclass in engineering logic. There is so much to learn from the way things were built to last, and those lessons help me create more resilient solutions for the future. I’m at my best in teams where communication is treated as a core tool and where trust is the foundation for everything we build together.

## Technical Skills
### Programming & Software Development
<div class="skill-tags">
<span class="skill-tag">C/C++</span>
<span class="skill-tag">Python</span>
<span class="skill-tag">C# / .NET</span>
<span class="skill-tag">Matlab</span>
<span class="skill-tag">SQL</span>
<span class="skill-tag">Git</span>
<span class="skill-tag">CMake</span>
<span class="skill-tag">CI/CD</span>
</div>

### Embedded & Industrial Systems
<div class="skill-tags">
<span class="skill-tag">Embedded Linux</span>
<span class="skill-tag">RTOS</span>
<span class="skill-tag">Yocto Project</span>
<span class="skill-tag">PLC (Beckhoff)</span>
<span class="skill-tag">ST (IEC 61131-3)</span>
<span class="skill-tag">VHDL</span>
<span class="skill-tag">Real-Time Systems</span>
<span class="skill-tag">LabVIEW</span>
</div>

### Hardware Engineering & Analysis
<div class="skill-tags">
<span class="skill-tag">Analog/Digital Design</span>
<span class="skill-tag">Schematic Analysis</span>
<span class="skill-tag">Eagle</span>
<span class="skill-tag">LTSpice</span>
<span class="skill-tag">Eplan</span>
<span class="skill-tag">Oscilloscopes & Logic Analyzers</span>
</div>

### Frameworks & UI
<div class="skill-tags">
<span class="skill-tag">Qt</span>
<span class="skill-tag">WPF / MVVM</span>
<span class="skill-tag">MFC</span>
<span class="skill-tag">MAUI</span>
</div>

### Systems & Research Methodology
<div class="skill-tags">
<span class="skill-tag">Control Theory</span>
<span class="skill-tag">Systems Engineering</span>
<span class="skill-tag">Requirements Engineering</span>
<span class="skill-tag">Data Analysis</span>
<span class="skill-tag">R&D Methodology</span>
</div>

## Professional Philosophy (Soft Skills)
<div class="skill-tags">
<span class="skill-tag">Interdisciplinary Collaboration</span>
<span class="skill-tag">Technical Communication</span>
<span class="skill-tag">Transparency</span>
<span class="skill-tag">Mentorship & Feedback</span>
<span class="skill-tag">Complex Problem Solving</span>
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