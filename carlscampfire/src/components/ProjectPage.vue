<template lang="html">
  <div class="pageContainer">
    <h1 class="pageHeading">PROJECTS</h1>
    <wordcloud
      :data="defaultWords"
      nameKey="name"
      valueKey="value"
      font="Bebas Neue"
      :fontSize="[30,50]"
      :rotate="{from: -45, to: 45, numOfOrientation: 2 }"
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
     myColors: ['#E3170A','#FFF', '#091540'],
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
  min-height: 60vh;
  height: auto;
  top: 0px;
  left: 0px;
  font-family: "Lato", sans-serif;
  background: linear-gradient(0deg, #00d2ff 0%, #3a47d5 100%);

}

.pageHeading {

  text-align: center;
  color: white;
  margin-bottom: 1em;
}
.wordcloud {
  width: 100%;
  height: 25em;

  background-image: url('../assets/clouds.jpg');
  background-size: 100% 100%;
  -webkit-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);

}
</style>
