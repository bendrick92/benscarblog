---
layout: default
url: /garage/wrx/
image: https://assets.bpwalters.com/images/bens_car_blog/wrx_door.jpg
title: WRX
mods:
- Weathertech floormats
- Grimmspeed front plate relocate
- 30% tint
- "[XPEL Ultimate paint protection film](/xpel-ultimate-review/)"
- "[Perrin Shift Stop](/perrin-shift-stop-review/)"
- "[Front & rear door sound deadening](/sound-deadening-the-wrx/)"
- "[Gloss black badging](/blacking-out-the-wrx/)"
- Enkei YS5 (17x7.5 +55) + General Altimax Arctic 12 (235/45R-17) (winter wheels & tires)
- "[Subiebros F1 rear fog light](/cleaning-up-the-rear-of-the-wrx/)"
- "[Subiebros LED license plate lights](/cleaning-up-the-rear-of-the-wrx/)"
- "[Carbon fiber e-brake handle](/carbon-e-brake-perrin-drift-button-review/)"
- "[Perrin Drift Button](/carbon-e-brake-perrin-drift-button-review/)"
- "[JDM dual console armrest](/jdm-dual-console-armrest-extension-review/)"
- "[Blacked out headlight housing, Morimoto D2S 4.0 HIDs, Diode Dynamics c-lights](/morimoto-d2s-4.0-hid-retrofit/)"
- "[Blacked out taillights, Diode Dynamics Tail as Turn module](/wrx-taillight-blackout/)"
- Diode Dynamics interior LEDs
- Morimoto LED foglights
- "[Bayson R V-Limited front lip](/bayson-r-lip-review/)"
- Billetworkz custom shift knob
- JDM coin tray
- JDM grocery hook
- "[Custom carbon-wrapped shifter trim](/diy-carbon-fiber)"
- Blacked out vent trim
- "[Rays Gram Lights 57DR (18x9.5 +38) + General G-MAX RS (255/35ZR-18)](/powder-coating-my-wheels)"
- HT Autos side skirts, rear spats
- OLM LED black turn signal housings
- "[COBB Accessport V3 w/ MAPerformance Stage 1 Tune](/cobb-accessport-review/)"
- "[KNS Brake Rotors w/ Hawk HPS 5.0 pads](/wrx-brake-upgrade)"
- COBB SS 3" cat-back exhaust
---

<section id="wrx" class="car">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/wrx_door.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1>{{ page.title }}</h1>
                </div>
            </div>
        </div>
    </section>
    <section id="history">
        <div class="container">
            <div class="item flex-100">
                <p><span class="is-first-letter">I</span>n early July 2017 I fulfilled a life-long dream and <a href="/buying-a-wrx">placed an order</a> for a 2018 WRX; a Premium in Lapis Blue Pearl.</p>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/wrx_dealership.jpg"></p>
                <p>The WRX neatly filled the void left when I sold my <a href="/garage/fiesta-st">Fiesta ST</a>, and proved itself to be a much more practical daily driver without sacrificing too many of the things that made the ST great.</p>
                <p>I had a great four and a half years with the WRX, but as I hit 30, I realized my priorities and interests were so different, I needed a car that better suited my, and my families needs. So in March 2022 I decided to <a href="/wrx-goodbye">trade in the WRX</a> for a <a href="/wrx-replacement">2022 Legacy Touring XT</a>.</p>
                <p>I'll always consider the WRX my "attainable dream car", and absolutely appreciated every day I was able to drive it!</p>
                <p>For more posts on the WRX, check out list below (in chronological order):</p>
                <ul>
                    {% for post in site.categories.wrx reversed %}
                        <li>
                            <a class="is-bold" href="{{ post.url }}" target="_blank">{{ post.title }}</a>
                        </li>
                    {% endfor %}
                </ul>
            </div>
        </div>
    </section>
    <section id="modifications">
        <div class="container">
            <div class="item flex-100">
                <h2 class="is-center-aligned">Modifications</h2>
                <p>My main focus when modding the WRX was to add refinement and features I felt were missing from the factory. While most of the mods were aesthetic, I did eventually do a few <a href="/cobb-accessport-review">performance mods</a>.</p>
                <p>Below is a complete list of mods with links to relevant posts:</p>
                <ul>
                    {% for mod in page.mods %}
                        <li>{{ mod | markdownify }}</li>
                    {% endfor %}
                </ul>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/cobb_accessport_review/summer_drive.jpg"></p>
            </div>
        </div>
    </section>
</section>