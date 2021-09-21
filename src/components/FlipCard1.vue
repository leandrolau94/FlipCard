<template>
    <div>
        <div class="front">
            <div class="front__top__right">
                <img class="pp1" v-bind:src="require('../pp1.jpg')">
            </div>
            <div class="front__down">
                <h1>Capolavoro Negosiazione</h1>
                <p>Lui e il capo dell'impresa. Prende
                    decizioni dificili e che possano
                    cambiare il cammino fino l'essito.
                    E molto bravo ed e riuscito a finire
                    qualche lavoro in cui c'e.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FlipCard1',
    props: {
        data1: String,
        msg1: String
    },
    data1(){
        return {
            miaImagine
        }
    }
}
</script>

<style>
.front {
    width: 200px;
    height: 300px;
    margin: 50px auto 50px;
    padding: 0;
    border: none;
    border-radius: 10% 10% 20% 20%;
    background-image: linear-gradient(to right, rgb(207, 241, 240), rgb(132, 238, 224), rgb(8, 214, 241));
    box-shadow: 0px 3px 18px 3px rgba(0, 0, 0, 0.5);
    cursor: pointer;
}
.front:hover {
    background-image: linear-gradient(to left, rgb(207, 241, 240), rgb(132, 238, 224), rgb(8, 214, 241));
}
.front__top__right {
    border: none;
    width: 60%;
    height: 30%;
    display: block;
    float: right;
    border-radius: 20% 60% 60% 50%;
    margin: 5px 40px 0 0;
    background-color: rgb(27, 60, 82);
}
.pp1 {
    display: block;
    float: left;
    width: 90px;
    height: 65px;
    margin: 10px auto 10px;
    border-radius: 15% 60% 15% 60%;
    border: 8px solid inherit;
    object-fit: cover;
}
.front__down {
    border: none;
    margin: 0;
    width: 100%;
    height: 70%;
    display: block;
    float: left;
    background-color: inherit;
    border-radius: 0 0 45% 45%;
}
.front__down > h1, p {
    font-size: 16px;
    margin: 15px 0px 15px 0px;
    color: rgb(27, 60, 82);
}
.front__down > h1 {
    font-size: 18px;
}
</style>