---
layout: default
url: /garage/wrx/
image: https://assets.bpwalters.com/images/bens_car_blog/wrx_1.jpg
title: WRX
current_mods:
- Weathertech floormats
- Grimmspeed front plate relocate
- 30% tint
- "[XPEL Ultimate paint protection film](/xpel-ultimate-review/)"
- "[Perrin Shift Stop](/perrin-shift-stop-review/)"
- "[Front & rear door sound deadening](/sound-deadening-the-wrx/)"
- "[Gloss black badging](/blacking-out-the-wrx/)"
- Enkei YS5 (17x7.5) + General Altimax Arctic 12 (235/45R17) (winter wheels & tires)
- "[Subiebros F1 rear fog light](/cleaning-up-the-rear-of-the-wrx/)"
- "[Subiebros LED license plate lights](/cleaning-up-the-rear-of-the-wrx/)"
- "[Carbon fiber e-brake handle](/carbon-e-brake-perrin-drift-button-review/)"
- "[Perrin Drift Button](/carbon-e-brake-perrin-drift-button-review/)"
- "[JDM dual console armrest](/jdm-dual-console-armrest-extension-review/)"
future_mods:
- RCE lowering springs
- Painted headlight housing, HID/c-light retrofit
- LED foglights
- Tail-as-turn
- Interior/exterior LEDs
- Alcantara interior accents
---

<section id="wrx" class="car">
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
            <div class="item flex-33 is-center-aligned">
                <h2>Purchased</h2>
                <h4 class="is-thin">September 2017</h4>
            </div>
            <div class="item flex-33">
                <h2 class="is-center-aligned">Current Mods</h2>
                <ul class="mods-list">
                {% for mod in page.current_mods %}
                    <li>{{ mod | markdownify }}</li>
                {% endfor %}
                </ul>
            </div>
            <div class="item flex-33">
                <h2 class="is-center-aligned">Future Mods</h2>
                <ul class="mods-list">
                {% for mod in page.future_mods %}
                    <li>{{ mod | markdownify }}</li>
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
                <p>In early July 2017 I fulfilled a life-long dream and <a href="/buying-a-wrx">placed an order</a> for a 2018 WRX; a Premium in Lapis Blue (no options).</p>
                <p>After 9 long weeks of waiting, I <a href="/taking-delivery-of-my-wrx">took delivery</a> of the car and immediately fell in love.  While I miss my Fiesta ST, the WRX has neatly filled the void and proven itself as a much more practical daily driver without sacrificing too many of the things that made the ST great.</p>
                <p>As of late December 2017, I've racked up a little over 6500 miles on the WRX!  Most recently it's carried our family through a number of cross-state roadtrips, and handled snowstorms like a boss.</p>
            </div>
            <div class="item flex-100 is-center-aligned">
                <img src="https://assets.bpwalters.com/images/bens_car_blog/wrx_salted.jpg">
            </div>
        </div>
    </section>
</section>