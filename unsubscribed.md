---
layout: default
---

<section id="unsubscribed">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/wrx_nighttime_1.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1>Thank You</h1>
                </div>
            </div>
        </div>
    </section>
    <section id="details">
        <div class="container">
            <div class="item flex-100">
                <h1>You've been unsubscribed!</h1>
                <p>Sorry to see you go!  You'll no longer be notified of new posts!</p>
                <div id="subscribe-prompt">
                    <form method="POST" action="http://formspree.io/subscribe@benscarblog.com">
                        <input type="hidden" name="email" id="subscribe-email">
                        <input type="hidden" name="message" value="Please add me to the Ben's Car Blog mailing list!">
                        <input type="hidden" name="_next" value="/subscribed/" id="subscribe-callback">
                        <p>If this was a mistake, and/or you've changed your mind, please click <input type="submit" value="here" class="is-link"> to resubscribe.</p>
                    </form>
                </div>
            </div>
        </div>
    </section>
</section>
<script type="text/javascript">
    var subscribePrompt = document.getElementById('subscribe-prompt');
    var subscribeEmail = document.getElementById('subscribe-email');
    var subscribeCallback = document.getElementById('subscribe-callback');
    var emailParam = getParameterByName('email');

    if (emailParam) {
        subscribePrompt.style.display = 'block';
        subscribeEmail.value = emailParam;
        subscribeCallback.value = subscribeCallback.value + '?email=' + emailParam;
    }
    else {
        window.location.href = '/';
    }

    function getParameterByName(name) {
        url = window.location.href;
        name = name.replace(/[\[\]]/g, "\\$&");
        var regex = new RegExp("[?&]" + name + "(=([^&#]*)|&|#|$)"),
            results = regex.exec(url);
        if (!results) return null;
        if (!results[2]) return '';
        return decodeURIComponent(results[2].replace(/\+/g, " "));
    }
</script>