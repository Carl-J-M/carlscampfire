<template lang="html">
  <div class="pageContainer">
    <h2 class="pageHeading">PROJECTS</h2>
    <wordcloud
      :data="defaultWords"
      nameKey="name"
      valueKey="value"
      font="Lato"
      :fontSize="[10,80]"
      :rotate="{from: -90, to: 90, numOfOrientation: 5 }"
      :color="myColors"
      :showTooltip="false"
      :wordClick="wordClickHandler"
      class="wordcloud">
      </wordcloud>
  </div>
</template>

<script>
import wordcloud from 'vue-wordcloud'
export default {
  components: {
   wordcloud
 },
 methods: {
   wordClickHandler(name, value, vm) {
     console.log('wordClickHandler', name, value, vm);
   }
 },
 data() {
   return {
     myColors: ['#E3170A', '#091540'],
     defaultWords: [
       {
         "name": "Travelbucket",
         "value": 0
       },
       {
         "name": "Cryptic",
         "value": 0
       },
       {
         "name": "Reddit 2.0",
         "value": 0
       },
       {
         "name": "Randomflix",
         "value": 0
       },
       {
         "name": "Reddit 2.0",
         "value": 0
       },
       {
         "name": "Reddit 2.0",
         "value": 0
       },
       {
         "name": "Reddit 2.0",
         "value": 0
       },
       {
         "name": "Reddit 2.0",
         "value": 0
       },
       {
         "name": "Reddit 2.0",
         "value": 0
       },
     ]
   }
  }
}
</script>

<style lang="css" scoped>
.pageContainer {
  display: flex;
  align-items: center;
  flex-direction: column;

  width: 100vw;
  min-height: 100vh;
  height: auto;
  top: 0px;
  left: 0px;
  font-family: "Lato", sans-serif;
  background: url('../assets/workshop.jpg');
  background-size: 100% 100%;
  background-repeat: no-repeat;
  /* background: linear-gradient(0deg, #00d2ff 0%, #3a47d5 100%); */

}

.pageHeading {

  text-align: center;
  color: white;
  background-color:  rgba(15, 155, 255);
  -webkit-box-shadow: 0px 0px 44px 16px rgba(0,0,0,0.75);
-moz-box-shadow: 0px 0px 44px 16px rgba(0,0,0,0.75);
box-shadow: 0px 0px 44px 16px rgba(0,0,0,0.75);
  height: 20vh;
  padding-top: 4%;
  width: 100%;

}
.wordcloud {
  width: 80%;
  height: 100vh;
  margin-top: 20px;
  margin-bottom: 20px;
  background-image: url('../assets/crumpled-paper.jpg');


}
</style>
