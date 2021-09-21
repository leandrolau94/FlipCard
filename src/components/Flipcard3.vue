<template>
    <div>
        <div class="presentation">
            <div class="presentation_top">
                <img src="./leo_picture.jpg" alt="picture">
                <h2>Leandro Lau</h2>
                <p>Graphic Designer</p>
            </div>
            <div class="presentation_bottom">
                <div class="phone">
                    <img src="./phone_24px.png" alt="phone">
                    <p>Phone</p><br>
                    <p>(+53) 5497-7890</p>
                </div>
                <div class="email">
                    <img src="./envelope_26px.png" alt="mail">
                    <p>Email Address</p><br>
                    <p>l1d9l9a4@gmail.com</p>
                </div>
                <div class="website">
                    <img src="./icons8_yelp_50px.png" alt="web">
                    <p>Website</p>
                    <p>www.lean-design-dro.com</p>
                </div>
                <div class="address">
                    <img src="./icons8_marker_24px.png" alt="address">
                    <p>Address</p><br>
                    <p>123 Main Street</p><br>
                    <p>California, USA 456789</p>
                </div>
                <div class="social_networks">
                    <img src="./icons8_facebook_24px.png" alt="facebook">
                    <img src="./icons8_twitter_24px.png" alt="twitter">
                    <img src="./icons8_whatsapp_30px.png" alt="whatsapp">
                    <img src="./icons8_telegram_app_50px.png" alt="telegram">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Flipcard3'
}
</script>

<style>
:root {
    --myprimary: #131392;
}
.presentation {
    width: 200px;
    height: 300px;
    margin: 50px auto 50px;
    padding: 0;
    border: none;
    box-shadow: 0px 3px 10px 3px rgba(27, 27, 27, 0.5);
    cursor: pointer;
    border-radius: 10px;
}
.presentation_top {
    background-color: var(--myprimary);
    border-radius: 10px 10px 0 0;
    display: block;
    float: left;
    width: 100%;
    height: 100px;
}
.presentation_top > img {
    width: 45px;
    height: 50px;
    margin-top: 5px;
    border-radius: 15px;
}
.presentation_top > h2 {
    color: white;
    font-weight: 400;
    font-size: 1.7vw;
}
.presentation_top > p {
    color: white;
    font-size: .8vw;
    margin-top: 0;
}
.presentation_bottom {
    background-color: #e6e6e6;
    margin-top: 0;
    display: block;
    float: left;
    width: 100%;
    height: 200px;
    border-radius: 0 0 10px 10px;
}
.phone, .email, .website, .social_networks {
    border: none;
    width: 90%;
    height: 31px;
    display: block;
    float: left;
    margin: 2.5px 10px 2.5px 10px;
    border-radius: 5px;
    background-color: #ffffff;
    text-align: center;
    align-items: center;
}
.address {
    border: none;
    width: 90%;
    height: 48px;
    display: block;
    float: left;
    margin: 2.5px 10px 2.5px 10px;
    border-radius: 5px;
    background-color: #ffffff;
}
.phone > img, .email > img, .website > img, .address > img, .social_networks > img {
    width: 25px;
    height: 25px;
    display: block;
    float: left;
    margin-left: 10px;
}
.phone > img, .email > img, .website > img {
    margin-top: 3px;
}
.address > img {
    margin-top: 10px;
}
.phone > p, .email > p, .website > p, .address > p {
    font-size: .8vw;
    display: block;
    float: left;
    margin: 0px 0px 0 3px;
}
img + p {
    color: var(--myprimary);
    font-weight: 600;
}
.address > p:last-child {
    margin-left: 38px;
}
.social_networks > img {
    width: 30px;
    height: 30px;
    margin-left: 12px;
}
.phone:hover, .email:hover, .address:hover, .website:hover, .social_networks:hover {
    background-color: lightsteelblue;
}
</style>