<template lang="html">
  <div class="pageContainer">
    <h1 class="pageHeading">Projects</h1>
    <wordcloud
      :data="defaultWords"
      nameKey="name"
      valueKey="value"
      font="Helvetica"
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

  background: #F7971E;  /* fallback for old browsers */
background: -webkit-linear-gradient(to bottom, #FFD200, #F7971E);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to bottom, #FFD200, #F7971E); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}

.pageHeading {

  text-align: center;

}
.wordcloud {
  width: 80%;
  height: 25em;
  background-color: rgba(255, 176, 0, 0.2);
  border-radius: 5px;


}
</style>
