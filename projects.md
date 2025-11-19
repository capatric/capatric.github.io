cat > projects.md << 'EOF'
---
layout: default
title: Projects
permalink: /projects/
---

<section>
    <h2>All Projects</h2>
    <ul class="project-list">
        {% for project in site.projects %}
        <li>
            <a href="{{ project.url }}" class="project-title">{{ project.title }}</a>
            <p class="project-meta">{{ project.type }} · {{ project.year }}</p>
            <p class="project-description">{{ project.description }}</p>
        </li>
        {% endfor %}
    </ul>
</section>
EOF
