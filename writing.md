cat > writing.md << 'EOF'
---
layout: default
title: Writing
permalink: /writing/
---

<section>
    <h2>All Writing</h2>
    <ul class="writing-list">
        {% assign sorted_writing = site.writing | sort: 'date' | reverse %}
        {% for post in sorted_writing %}
        <li>
            <span class="post-date">{{ post.date | date: "%b %Y" }}</span>
            <a href="{{ post.url }}" class="post-title">{{ post.title }}</a>
            <p class="post-description">{{ post.description }}</p>
        </li>
        {% endfor %}
    </ul>
</section>
EOF
