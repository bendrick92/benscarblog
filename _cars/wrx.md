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
- KNS Brake Rotors w/ Hawk HPS 5.0 pads
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
                <p><span class="is-first-letter">I</span>n early July 2017 I fulfilled a life-long dream and <a href="/buying-a-wrx">placed an order</a> for a 2018 WRX; a Premium in Lapis Blue Pearl.  After 9 long weeks of waiting, I <a href="/taking-delivery-of-my-wrx">took delivery</a> of the car!</p>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/wrx_dealership.jpg"></p>
                <p>While I still miss my Fiesta ST, the WRX has neatly filled that void and proven itself to be a much more practical daily driver without sacrificing too many of the things that made the ST great.</p>
                <p>As of September 2018, I've racked up a little over 19,000 miles on the WRX!  I recently completed an <a href="/morimoto-d2s-4.0-hid-retrofit">HID retrofit</a> and <a href="/wrx-taillight-blackout">taillight blackout</a>, which totally transformed the exterior!</p>
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
                <p>My main focus in modding the WRX has been to add refinement and features I've felt were missing from the factory.  While most of the mods have been aesthetic up to this point, I do plan to add a bit of power down the road.  For now, I'll enjoy that warranty while I still can! ;)</p>
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