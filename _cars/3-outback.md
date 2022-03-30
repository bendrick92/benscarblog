---
layout: default
url: /garage/outback/
image: https://assets.bpwalters.com/images/bens_car_blog/outback.jpg
title: Outback
---

<section id="outback" class="car">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/outback.jpg');"></div>
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
                <p><span class="is-first-letter">S</span>hortly after graduating college, my wife's old Mercury Sable stranded itself in a grocery store parking lot thanks to some unfixable electrical issues. Her next car, a 2012 Ford Focus, was a quick fix solution to our one car problem. Unfortunately, that car had issues of it's own that left us in a tricky position - do we get rid of the Focus and pick up another potentially short-lived replacement?</p>
                <p>We had thrown around the idea of picking up an Outback or Forester for her down the road, and actually test drove used copies of both one weekend long before we were looking to actually pull the trigger. We decided that an Outback would be the perfect next car for her, and would easily suit us well for many years to come.</p>
                <p>Trying to be responsible adults, we had the best intentions of milking the most out of her problematic Focus as we could. As winter rapidly approached however, we both felt that putting up with that car for another season would be more stress-inducing than it was worth. So we explored our options and ended up finding a super clean 2017 Outback Premium through CarMax.</p>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/outback_badge.jpg"/></p>
                <p>Since picking up the car in the Fall of 2019, we have enjoyed every mile behind the wheel. Its proven to be an extremely capable family hauler, the driving position is perfect for my wife's preference, and the smooth ride combined with the Eyesight cruise control means its perfect for long distance trips!</p>
                <p><img src="https://assets.bpwalters.com/images/bens_car_blog/outback_interior.jpg"/></p>
                <p>For more posts on the Outback, check out list below (in chronological order):</p>
                <ul>
                    {% for post in site.categories.outback reversed %}
                        <li>
                            <a class="is-bold" href="{{ post.url }}" target="_blank">{{ post.title }}</a>
                        </li>
                    {% endfor %}
                </ul>
            </div>
        </div>
    </section>
</section>