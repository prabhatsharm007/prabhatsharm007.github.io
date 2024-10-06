---
layout: default
title: Home
---

<div class="hero-section">
    <!-- <img src="/assets/img/default.png" alt="Clinical Bytes Logo" class="hero-logo"> -->
    <p>{{ site.description }}</p>
</div>

<div class="recent-blogs">
    <h2>Recent Posts</h2>
    <div class="row">
        {% for post in site.posts limit:3 %}
        <div class="col-md-4">
            <div class="card mb-4">
                <div class="card-body">
                    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
                    <p>{{ post.excerpt }}</p>
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</div>
