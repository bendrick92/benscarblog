---
layout: default
url: /garage/cougar/
image: https://assets.bpwalters.com/images/bens_car_blog/cougar_2.jpg
title: Cougar
mods:
- AEM intake
- Custom Magnaflow catback exhaust
- Roush spoiler
- Alpine head unit, speakers
---

<section id="cougar" class="car">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/cougar_1.jpg');"></div>
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
                <p><span class="is-first-letter">E</span>veryone remembers their first car.  Everything about it was just so exciting!  The sense of freedom, ownership, responsibility...  I had it set in my mind that I wanted a WRX.  Unfortunately, insurance rates and my limited budget brought me back to reality pretty quickly.  However, the car I ended up in is one I'll never forget - a low mileage, silver, five speed 2000 Mercury Cougar.</p>
                <p>The car was in great shape for being over nine years old!  A local used dealership had been searching for a car for me, and the Cougar popped up in an auction down in Illinois in late 2009.  I didn't know much about the car at the time - the "New Edge" Cougar models ('99-'02) didn't sell in huge numbers.  Fortunately an active community over on the <a href="http://www.newcougar.org">NECO forums</a> provided a wealth of information about the car.</p>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/cougar_3.jpg"></p>
                <p>The Cougar served me faithfully all the way through college, but began to show its age in late 2013.  With corrosion starting to surface and frequent alternator issues (a documented issue with that generation) I made the decision to upgrade to the Fiesta ST shortly after graduating in 2014.</p>
                <p>In spite of its issues, I miss this car.  It was an awesome highway cruiser.  Even with the exhaust, I never found myself fatigued by drone, a rough ride, or cramped cabin.  Being a coupe meant it felt much more spacious than it actually was!  Combine that with a HUGE trunk (it's actually a hatchback) and it served as a suprisingly practical daily driver.</p>
            </div>
        </div>
    </section>
    <section id="modifications">
        <div class="container">
            <div class="item flex-100">
                <h2 class="is-center-aligned">Modifications</h2>
                <p>I made the most of my part-time McDonald's paycheck and managed to save up for a few cosmetic mods like as a Roush spoiler, and tail light covers.  In addition, I ponied up the cash for a custom Magnaflow catback exhaust.  Being a V6 model, I was pleasantly suprised at the sounds it made!</p>
                <ul>
                    {% for mod in page.mods %}
                        <li>{{ mod | markdownify }}</li>
                    {% endfor %}
                </ul>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/cougar_2.jpg"></p>
            </div>
        </div>
    </section>
</section>