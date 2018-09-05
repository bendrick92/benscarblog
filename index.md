---
layout: default
pagination:
    enabled: true
---

<section id="homepage">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/nardi.jpg');"></div>
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
    {% if paginator.previous_page %}
        <section id="posts">
            <div class="container">
                {% for post in paginator.posts offset: 2 %}
                    <div class="item flex-50">
                        {% include post_preview.html %}
                    </div>
                {% endfor %}
            </div>
        </section>
    {% else %}
        <section id="latest-post">
            <div class="container">
                <div class="item flex-100 is-center-aligned">
                    <h1>What's New</h1>
                </div>
                {% for post in paginator.posts offset: 1 limit: 1 %}
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
                    <h1>Latest Posts</h1>
                </div>
                {% for post in paginator.posts offset: 2 %}
                    <div class="item flex-50">
                        {% include post_preview.html %}
                    </div>
                {% endfor %}
            </div>
        </section>
    {% endif %}
    {% if paginator.total_pages > 1 %}
        <section id="pagination" class="is-center-aligned">
            <div class="container">
                <div class="item flex-100">
                    <ul class="is-pagination-list">
                    {% if paginator.page_trail %}
                        {% if paginator.previous_page %}
                            <li><a href="{{ paginator.previous_page_path | prepend: site.baseurl }}">&lt;</a></li>
                        {% endif %}
                        {% for trail in paginator.page_trail %}
                            <li>
                                {% assign page_url = page.url | remove: ".html" | remove: "index" %}
                                {% assign trail_path = trail.path | remove: 'index.html' %}
                                {% if page_url == trail_path %}
                                    <a href="#" class="curr-page">{{ trail.num }}</a>
                                {% else %}
                                    <a href="{{ trail.path | prepend: site.baseurl | remove: 'index.html' }}">{{ trail.num }}</a>
                                {% endif %}
                            </li>
                        {% endfor %}
                        {% if paginator.next_page %}
                            <li><a href="{{ paginator.next_page_path | prepend: site.baseurl }}">&gt;</a></li>
                        {% endif %}
                    {% endif %}
                    </ul>
                </div>
            </div>
        </section>
    {% endif %}
</section>