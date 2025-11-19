cat > index.md << 'EOF'
---
layout: default
title: Home
---

<section>
    <p class="intro">
        I'm interested in the intersection of technology, philosophy, and human potential. 
        I write about ideas that fascinate me and build things that solve problems I care about.
    </p>
</section>

<section id="writing">
    <h2>Recent Writing</h2>
    <ul class="writing-list">
        {% assign sorted_writing = site.writing | sort: 'date' | reverse %}
        {% for post in sorted_writing limit:3 %}
        <li>
            <span class="post-date">{{ post.date | date: "%b %Y" }}</span>
            <a href="{{ post.url }}" class="post-title">{{ post.title }}</a>
            <p class="post-description">{{ post.description }}</p>
        </li>
        {% endfor %}
    </ul>
    <p style="text-align: center; margin-top: 40px;">
        <a href="/writing" style="color: #555; text-decoration: none; border-bottom: 1px solid #555;">View all writing →</a>
    </p>
</section>

<section id="projects">
    <h2>Selected Projects</h2>
    <ul class="project-list">
        {% for project in site.projects limit:3 %}
        <li>
            <a href="{{ project.url }}" class="project-title">{{ project.title }}</a>
            <p class="project-meta">{{ project.type }} · {{ project.year }}</p>
            <p class="project-description">{{ project.description }}</p>
        </li>
        {% endfor %}
    </ul>
    <p style="text-align: center; margin-top: 40px;">
        <a href="/projects" style="color: #555; text-decoration: none; border-bottom: 1px solid #555;">View all projects →</a>
    </p>
</section>

<footer>
    <p>Built with care. No analytics, no tracking.</p>
</footer>
EOF
