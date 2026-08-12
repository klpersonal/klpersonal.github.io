---
layout: default
title: Home
---

<section class="hero">
  <p class="eyebrow">Welcome</p>
  <h1>Your Name</h1>
  <p class="lead">
    I am a researcher / professional working on topics such as
    <strong>Topic One</strong>, <strong>Topic Two</strong>, and <strong>Topic Three</strong>.
  </p>
  <p>
    This website contains my publications, CV, occasional writing, and other
    information about my work.
  </p>
  <div class="actions">
    <a class="button" href="{{ '/publications/' | relative_url }}">View publications</a>
    <a class="button button-secondary" href="{{ '/cv/' | relative_url }}">View CV</a>
  </div>
</section>

<section>
  <h2>Recent writing</h2>
  {% if site.posts.size > 0 %}
  <div class="card-list">
    {% for post in site.posts limit:3 %}
      <article class="card">
        <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      </article>
    {% endfor %}
  </div>
  {% else %}
  <p>No posts yet.</p>
  {% endif %}
</section>
