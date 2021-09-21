<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <!--<router-view/>-->
    <div id="mainCard__container">
      <footer id="footer">
        <FlipCard id="flip1" msg="id1"/>
        <FlipCard id="flip2" msg="id2"/>
        <FlipCard id="flip3" msg="id3"/>
      </footer>
      <footer id="footer1">
        <FlipCard1 id="flip4"/>
        <FlipCard1 id="flip5"/>
        <FlipCard1 id="flip6"/>
      </footer>
      <footer id="footer2">
        <Flipcard2 id="flip7" />
        <Flipcard2 id="flip8" />
        <Flipcard2 id="flip9" />
      </footer>
    </div>
  </div>
</template>

<script>
import FlipCard from './components/Flipcard.vue';
import FlipCard1 from './components/FlipCard1.vue';
import Flipcard2 from './components/Flipcard2.vue'
export default {
  name: 'App',
  components: {
    FlipCard,
    FlipCard1,
    Flipcard2
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /*margin-top: 60px;*/
}
#mainCard__container {
  width: 98%;
  height: auto;
  margin: 0% 1%;
  border: none;
  display: block;
  float: left;
}
#footer, #footer1, #footer2 {
  border: none;
  display: block;
  float: left;
  width: 90%;
  height: auto;
  margin: 0% 4%;
}
#flip1, #flip2, #flip3, #flip4, #flip5, #flip6, #flip7, #flip8, #flip9 {
  display: block;
  float: left;
  margin: 0% 8% 0% 8%;
}
#footer {
  background-image: linear-gradient(to bottom left,#FFCE00, #FE4880, #F3F3F3);
}
#footer1 {
  background-image: linear-gradient(to right, rgb(207, 241, 240), rgb(132, 238, 224), rgb(8, 214, 241));;
}
#footer2 {
  background-image: linear-gradient(to right, #a1caff, #6a95cc, #3a4d8f, #132665, #332b3a);
}
</style>