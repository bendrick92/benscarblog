---
layout: default
---

<section id="unsubscribe">
    <section id="intro" class="is-intro-section">
        <div class="background-image-wrapper is-dark">
            <div class="is-opaque" style="background-image: url('https://assets.bpwalters.com/images/bens_car_blog/wrx_nighttime_1.jpg');"></div>
        </div>
        <div class="container has-middle-text">
            <div class="item flex-100">
                <div class="intro-title">
                    <h1>Unsubscribe</h1>
                </div>
            </div>
        </div>
    </section>
    <section id="details">
        <div class="container">
            <div class="item flex-100 is-center-aligned">
                <h1>Sorry to see you go!</h1>
                <p>No longer want to receive emails?</p>
                <form method="POST" onsubmit="return unsubscribe();" id="unsubscribe-form">
                    <div class="validation-wrapper">
                        <span id="unsubscribe-email-validation" class="is-validation-message"></span>
                        <input type="email" name="email" placeholder="Your email" id="unsubscribe-email">
                    </div>
                    <input type="hidden" name="message" value="Please REMOVE me from the Ben's Car Blog mailing list!">
                    <input type="hidden" name="_next" value="/unsubscribed/" id="unsubscribe-callback">
                    <input type="text" name="_gotcha" style="display: none;">
                    <button type="submit">Unsubscribe</button>
                </form>
            </div>
        </div>
    </section>
</section>
<script type="text/javascript">
    var unsubscribeForm =  document.getElementById('unsubscribe-form');
    unsubscribeForm.setAttribute('action', '//formspree.io/' + 'unsubscribe' + '@' + 'benscarblog' + '.' + 'com');

    function unsubscribe() {
        var unsubscribeEmailValidation = document.getElementById('unsubscribe-email-validation');
        var unsubscribeEmail = document.getElementById('unsubscribe-email');
        var unsubscribeCallback = document.getElementById('unsubscribe-callback');

        if (validateEmail(unsubscribeEmail.value)) {
            unsubscribeCallback.value = unsubscribeCallback.value + '?email=' + unsubscribeEmail.value;
            return true;
        }
        else {
            unsubscribeEmail.style.border = '1px solid #F00';
            unsubscribeEmailValidation.innerHTML = 'Please enter a valid email';
            return false;
        }

        function validateEmail(email) {
            var re = /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
            return re.test(email.toLowerCase());
        }
    }
</script>