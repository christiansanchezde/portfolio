---
layout: default
---

## About Me
I am a Senior R&D Software Engineer with a passion for bridging the gap between research and production. My work focuses on optimizing neural networks for edge devices and building scalable distributed systems.

Currently, I am working on **High Performance Computing** solutions at [Company Name]. Previously, I conducted research on Computer Vision at [University/Lab].

## Technical Skills
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

## Selected Publications
<div class="pub-item">
    <span class="pub-title">Optimizing Transformer Inference on Edge Devices</span>
    <span class="pub-meta">IEEE Conference on Computer Vision, 2023</span>
</div>
<div class="pub-item">
    <span class="pub-title">A Distributed Protocol for IoT Mesh Networks</span>
    <span class="pub-meta">Journal of Network Systems, 2022</span>
</div>

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