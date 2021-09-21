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
    </div>
  </div>
</template>

<script>
import FlipCard from './components/Flipcard.vue';
import FlipCard1 from './components/FlipCard1.vue';

export default {
  name: 'App',
  components: {
    FlipCard,
    FlipCard1
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
  border: solid;
  display: block;
  float: left;
}
#footer {
  border: solid;
  display: block;
  float: left;
  width: 90%;
  height: auto;
  margin: 0% 4%;
  background-image: linear-gradient(to bottom left,#FFCE00, #FE4880, #F3F3F3);
}
#flip1, #flip2, #flip3, #flip4, #flip5, #flip6 {
  display: block;
  float: left;
  margin: 0% 8% 0% 8%;
}
#footer1 {
  border: solid;
  display: block;
  float: left;
  width: 90%;
  height: auto;
  margin: 0% 4%;
  background-image: linear-gradient(to right, rgb(207, 241, 240), rgb(132, 238, 224), rgb(8, 214, 241));;
}
</style>
