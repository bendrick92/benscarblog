---
layout: default
pagination:
    enabled: true
---

<section id="homepage">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/fiesta_1.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1 class="is-hidden-mobile is-hidden-tablet"><span>Ben's</span> Car Blog</h1>
                    <h1 class="is-hidden-desktop"><span>Ben's</span><br>Car Blog</h1>
                    <p class="is-subheading">Reviews, How-Tos, Everything Cars</p>
                </div>
            </div>
        </div>
    </section>
    <section id="latest-posts">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>Latest Posts</h1>
            </div>
            {% for post in paginator.posts %}
                <div class="item flex-50 has-gutter">
                    {% include post_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
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