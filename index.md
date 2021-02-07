---
layout: default
pagination:
    enabled: true
---

<section id="homepage">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/wrx_bridge.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1 class="is-hidden-mobile is-hidden-tablet"><span>Ben's</span> Car Blog</h1>
                    <h1 class="is-hidden-desktop"><span>Ben's</span><br>Car Blog</h1>
                </div>
            </div>
        </div>
    </section>
    <section id="whats-new">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>New Stuff</h1>
            </div>
            {% for post in site.posts limit: 2 %}
                <div class="item flex-50">
                    {% include post_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
    {% include subscribe_section.html %}
    <section id="popular">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>Popular Stuff</h1>
            </div>
            {% assign featured_posts = site.posts | where:"featured", "true" %}
            {% for post in featured_posts %}
                <div class="item flex-50">
                    {% include post_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
    {% include support_section.html %}
    <section id="other-stuff">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>Other Stuff</h1>
            </div>
            {% for post in site.posts offset: 2 %}
                <div class="item flex-50">
                    {% include post_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
</section>