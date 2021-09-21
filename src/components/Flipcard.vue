<template>
    <div>
        <div class="card">
            <div class="card__inner" v-bind:id="msg" v-on:click="flip">
                <div class="card__face card__face--front">
                    <div class="aligned one">
                        <h2>Web Developer</h2>
                    </div>
                    <div class="aligned two">
                        <h3>E-mail:</h3>
                    </div>
                    <div class="aligned three">
                        <h4>leandro@icimaf.cu</h4>
                    </div>
                    <div class="aligned four">
                        <h3>Phone-Number:</h3>
                    </div>
                    <div class="aligned five">
                        <h4>(+53)54977890</h4>
                    </div>
                    <div class="aligned six">
                        <h3>Contact him at:</h3>
                    </div>
                    <div class="aligned seven">
                        <h4>http://www.web/leo-designes.org</h4>
                    </div>
                </div>
                <div class="card__face card__face--back">
                    <div class="card__content">
                        <div class="card__header">
                            <img class="pp" :src="myImage">
                            <h2>Leandro Lau</h2>
                        </div>
                        <div class="card__body">
                            <h3>JavaScript Vue.js</h3>
                            <p>Leandro is an enthusiastic web developer focusing
                                on JavaScript and Vue.js developements for
                                web page design. He graduated from Pure Math
                                at Havana University and learned programming
                                autodidactic.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import myImage from '../assets/pp.jpg';

export default {
    name: 'FlipCard',
    props: {
        data: String,
        msg: String
    },
    data(){
        return {
            myImage
        }
    },
    methods: {
        flip() {
            document.getElementById(this.msg).classList.toggle("is__flipped");
        }
    }
}
</script>

<style>
:root {
    --primary: #FFCE00;
    --secondary: #FE4880;
    --dark: #212121;
    --light: #F3F3F3;
}
* {
    margin: 0;
    padding: 0;
}
.card {
    margin: 50px auto 50px;
    width: 200px;
    height: 300px;
    perspective: 1000px;
}
.card__inner {
    width: 100%;
    height: 100%;
    transition: transform 1s;
    transform-style: preserve-3d;
    cursor: pointer;
    position: relative;
}
.is__flipped {
    transform: rotateY(180deg);
}
.card__face {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
    overflow: hidden;
    border-radius: 14px;
    box-shadow: 0px 3px 18px 3px rgba(0, 0, 0, 0.5);
}
.card__face--front {
    background-image: linear-gradient(to bottom right, var(--primary), var(--secondary));
    display: flex;
    align-items: center;
    justify-content: center;
}
.aligned {
    display: block;
    float: left;
    position: absolute;
    margin: 5px;
}
.one {
    top: 0%;
}
.two {
    top: 15%;
}
.three {
    top: 25%;
}
.four {
    top: 40%;
}
.five {
    top: 50%;
}
.six {
    top: 65%;
}
.seven {
    top: 75%;
}
.card__face--front .aligned h2 {
    color: #FFF;
    font-size: 20px;
    padding: 5px;
}
.card__face--front .aligned h3 {
    color: var(--light);
    font-size: 15px;
    padding: 5px;
}
.card__face--front .aligned h4 {
    color: var(--light);
    font-size: 12px;
    padding: 5px;
}
.card__face--front .aligned h4:hover {
    color: var(--dark);
    text-decoration: underline;
}
.card__face--back {
    background-color: var(--dark);
    transform: rotateY(180deg);
}
.card__content {
    width: 100%;
    height: 100%;
}
.card__header {
    position: relative;
    padding: 10px 10px 20px;
}
.card__header::after {
    content: '';
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: -1;
    border-radius: 0 0 50% 0;
    background-image: linear-gradient(to bottom left, var(--primary) 10%, var(--secondary) 115%);
}
.pp {
    display: block;
    width: 65px;
    height: 65px;
    margin: 0 auto 10px;
    border-radius: 50%;
    background-color: #FFF;
    border: 3px solid #FFF;
    object-fit: cover;
}
.card__header > h2 {
    color: #FFF;
    font-size: 20px;
    font-weight: 600;
    text-transform: uppercase;
    text-align: center;
}
.card__body {
    padding: 10px;
    background-color: var(--dark);
}
.card__body > h3 {
    color: var(--light);
    font-size: 18px;
    font-weight: 600;
    margin-bottom: 5px;
}
.card__body > p {
    color: var(--light);
    font-size: 12px;
    line-height: 1.5;
}
</style>