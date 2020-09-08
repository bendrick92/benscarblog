---
layout: default
pagination:
    enabled: true
---

<section id="homepage">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/xpel_ultimate_long_term/wrx_bumper.jpg');"></div>
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
    <section id="latest-post">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>What's New</h1>
            </div>
            {% for post in site.posts limit: 1 %}
                <div class="item flex-100 first-post">
                    {% include post_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
    {% include subscribe_section.html %}
    <section id="other-posts">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>Other Posts</h1>
            </div>
            {% for post in site.posts offset: 1 %}
                <div class="item flex-50">
                    {% include post_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
    {% include support_section.html %}
</section>