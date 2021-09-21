<template>
    <div>
        <div class="CARD">
            <div class="top">
                <div class="presentation_name">
                    <h3>Leandro Lau</h3>
                    <p>Web Designer</p>
                </div>
                <div class="heaxagon first"></div>
                <div class="heaxagon second"></div>
                <div class="heaxagon third"></div>
            </div>
            <div class="down">
                <div class="company_contact">
                    <p>COMPANY CONTACT<br>INFORMATION</p>
                </div>
                <div class="company_email">
                    <img src="./icons8_send_email_30px.png" alt="">
                    <p>webtrully@gmail.com</p>
                </div>
                <div class="company_phone">
                    <img src="./icons8_phone_30px.png" alt="">
                    <p>(+53) 5497-7890<br>(+53) 5389-9692</p>
                </div>
                <div class="home">
                    <img src="./icons8_home_page_24px.png" alt="">
                    <p>Vedado, Habana, Cuba</p>
                </div>
                <div class="company_web">
                    <img src="./icons8_globe_32px.png" alt="">
                    <a href="#" target="_blank">www.webtrully/ldla-94.design</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Flipcard2'
}
</script>

<style>
.CARD {
    width: 200px;
    height: 300px;
    margin: 50px auto 50px;
    padding: 0;
    border: none;
    background-image: linear-gradient(to bottom, #355c7d, #725a7a, #c56c86, #ff7582);
    box-shadow: 0px 3px 18px 3px rgba(0, 0, 0, 0.5);
    cursor: pointer;
}
.top, .down {
    width: 100%;
    border: none;
}
.top {
    height: 110px;
}
.down {
    height: 240px;
}
.top > .presentation_name {
    width: 100%;
    height: 50px;
}
.top > .presentation_name > h3 {
    font-weight: .5vw;
    color: #ffffff;
    margin: 0;
}
.top > .presentation_name > p {
    font-size: 1vw;
    color: rgb(148, 148, 148);
    margin: 0;
}
.heaxagon {
    border-bottom: 5px solid #6a95cc;
    border-top: 5px solid #6a95cc;
    width: 35px;
    height: 50px;
    display: block;
    float: left;
    position: absolute;
    margin-left: 85px;
}
.third {
    transform: rotateZ(90deg);
}
.first {
    transform: rotateZ(30deg);
}
.second {
    transform: rotateZ(-30deg);
}
.company_contact, .company_email, .company_phone, .home, .company_web {
    margin: 0 7%;
    padding: 0;
    text-align: center;
    width: 86%;
    height: 35px;
    border: none;
}
.down > .company_contact > p {
    font-size: 1vw;
    color: #ffffff;
    margin-top: 0;
}
.company_email > img, .company_phone > img, .home > img, .company_web > img {
    width: 30px;
    height: 30px;
    display: block;
    float: left;
}
.company_email > img:hover, .company_phone > img:hover, .home > img:hover, .company_web > img:hover {
    background-color: #355c7d;
    border-radius: 10%;
}
.company_email > p, .company_phone > p, .home > p, .company_web > a {
    font-size: .8vw;
    color: #ffffff;
    margin-top: 5px;
    display: block;
    float: right;
}
.company_web > a:hover {
    color: #355c7d;
}
.company_email > p {
    margin-right: 27px;
}
.company_phone > p {
    margin-right: 60px;
}
.home > p {
    margin-right: 24px;
}
</style>