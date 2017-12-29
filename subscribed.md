---
layout: default
---

<section id="subscribed">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/wrx_interior_1.jpg');"></div>
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
                <h1>You've been subscribed!</h1>
                <p>Thank you for signing up!  You'll be the first to be notified every time a new post goes live!</p>
                <div id="unsubscribe-prompt">
                    <form method="POST" action="http://formspree.io/unsubscribe@benscarblog.com">
                        <input type="hidden" name="email" id="unsubscribe-email">
                        <input type="hidden" name="message" value="Please remove me to the Ben's Car Blog mailing list!">
                        <input type="hidden" name="_next" value="/unsubscribed/" id="unsubscribe-callback">
                        <p>If you change your mind, please click <input type="submit" value="here" class="is-link"> to unsubscribe at any time.</p>
                    </form>
                </div>
            </div>
        </div>
    </section>
</section>
<script type="text/javascript">
    var unsubscribePrompt = document.getElementById('unsubscribe-prompt');
    var unsubscribeEmail = document.getElementById('unsubscribe-email');
    var unsubscribeCallback = document.getElementById('unsubscribe-callback');
    var emailParam = getParameterByName('email');

    if (emailParam) {
        unsubscribePrompt.style.display = 'block';
        unsubscribeEmail.value = emailParam;
        unsubscribeCallback.value = unsubscribeCallback.value + '?email=' + emailParam;
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