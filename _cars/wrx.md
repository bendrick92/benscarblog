---
layout: default
url: /garage/wrx/
image: https://assets.bpwalters.com/images/bens_car_blog/wrx_1.jpg
title: WRX
mods:
- Grimmspeed front plate relocate
---

<section id="fiesta-st">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/wrx_1.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1>{{ page.title }}</h1>
                </div>
            </div>
        </div>
    </section>
    <section id="details">
        <div class="container">
            <div class="item flex-50 is-center-aligned">
                <h2>Purchased</h2>
                <h4 class="is-thin">September 2017</h4>
            </div>
            <div class="item flex-50">
                <h2 class="is-center-aligned">Mods</h2>
                <ul>
                {% for mod in page.mods %}
                    <li>{{ mod }}</li>
                {% endfor %}
                </ul>
            </div>
        </div>
    </section>
    <section id="history">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h2>History</h2>
                <img src="https://assets.bpwalters.com/images/bens_car_blog/wrx_dealership.jpg">
            </div>
            <div class="item flex-100">
                <p>In early July 2017 I fulfilled a life-long dream and <a href="/buying-a-wrx">placed an order</a> for a 2018 WRX; specifically a Premium in Lapis Blue (no options).</p>
                <p>After 9 long weeks of waiting, I took delivery of the car and immediately fell in love.  While I miss my ST dearly, the WRX has already proven to be a much more practical daily driver.</p>
                <p>Plans for the car include a full overhaul of the stock headlights (HID retrofit, C-light upgrade, etc.), some basic interior improvements, as well as minor exterior cosmetic mods for now.  For at least the first year, I plan to keep the mods to a minimum.  Famous last words, right?</p>
            </div>
        </div>
    </section>
</section>