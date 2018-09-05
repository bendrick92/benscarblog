---
layout: default
url: /garage/fiesta-st/
image: https://assets.bpwalters.com/images/bens_car_blog/fiesta_1.jpg
title: Fiesta ST
mods:
- Rally Armor mudflaps
- COBB drop-in filter
- MAP catback exhaust
- Boomba shifter bracket bushings
- Mountune Quick Shift
- "[Custom front plate mount](/diy-fiesta-focus-st-front-plate-relocate/)"
- "[RAAMAudio sound deadening](/sound-deadening-the-fiesta-st/)"
---

<section id="fiesta-st" class="car">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/fiesta_1.jpg');"></div>
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
                <p><span class="is-first-letter">A</span>fter graduating college in the summer of 2014, I found myself searching for a replacement for my 2000 Mercury Cougar.  Unpredictable alternator issues and a new full-time job left me wanting for something more reliable and preferably turbocharged.  I spent a few weeks looking at used STIs, WRXs, etc. but in the end I found myself behind the wheel of a practically new (1,971 miles on the odometer) 2014 Fiesta ST.</p>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/fiesta_st_front.jpg"></p>
                <p>The ST served as my daily driver for a little over three years until it was sold to a good friend in September 2017.  Overall, my three years with the ST were overwhemingly enjoyable and trouble free.  For more details on the Fiesta ST, feel free to check out my full <a href="/ford-fiesta-st-long-term-review" target="_blank">long term review</a>!</p>
            </div>
        </div>
    </section>
    <section id="modifications">
        <div class="container">
            <div class="item flex-100">
                <h2 class="is-center-aligned">Modifications</h2>
                <p>Overall, I made a few minor performance mods to the Fiesta ST, but stayed focused on retaining the factory warranty.  I never really sunk a ton of money into the vehicle, as I had always planned to upgrade to a WRX at some point in the future.</p>
                <ul>
                    {% for mod in page.mods %}
                        <li>{{ mod | markdownify }}</li>
                    {% endfor %}
                </ul>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/fiesta_2.jpg"></p>
            </div>
        </div>
    </section>
</section>