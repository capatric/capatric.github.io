---
layout: default
title: Home
---

# Hello, I'm [Your Name]

I'm a [your profession] focused on [your focus areas]. Currently [what you're doing now].

## What I Do

I specialize in building [description of your work]. My interests include [list 2-3 key interests].

## Recent Posts

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[View all posts →](/posts)

## Get in Touch

Feel free to reach out via [email](mailto:{{ site.email }}) or connect with me on [Twitter](https://twitter.com/yourhandle) / [LinkedIn](https://linkedin.com/in/yourprofile).
