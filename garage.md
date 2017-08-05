---
layout: default
---

<section id="garage">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/garage.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1>Garage</h1>
                </div>
            </div>
        </div>
    </section>
    <section id="car-list">
        <div class="container">
            {% for car in site.cars %}
                <div class="item flex-50 has-gutter">
                    {% include car_preview.html %}
                </div>
            {% endfor %}
        </div>
    </section>
</section>