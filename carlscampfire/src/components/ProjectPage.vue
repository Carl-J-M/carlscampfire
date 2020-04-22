<template lang="html">
  <div class="pageContainer">
    <h2 class="pageHeading">PROJECTS</h2>
    <div class="projectContainer">
        <div class="overlayOne pulseElement"/>
      <div class="project front">
         <h4>Cryptic</h4>
         <p>Puzzle app with admin login and secret event location map.</p>
      </div>
      <div class="overlayTwo pulseElement12"/>
      <div class="project front">
         <h4>Reddit 2.0</h4>
         <p>Vue.js app utilising the reddit API to retrieve posts from a typed subreddit, no page refresh.</p>
      </div>
      <div class="overlayThree pulseElement14"/>
      <div class="project front">
         <h4>TravelBucket</h4>
         <p>Ruby/Sinatra application using restful routes to retrieve data from a postgres SQL database. Travel bucket list application with CRUD functionality.</p>
      </div>
      <div class="overlayFour pulseElement16"/>
      <div class="project front">
         <h4>Randomflix</h4>
         <p>A simple film randomizer to help break the stalemate with my flatmates about what movie to watch.</p>
      </div>
    </div>
  </div>
</template>

<script>

export default {


}
</script>

<style lang="css" scoped>
.pageContainer {
  display: flex;
  align-items: center;
  flex-direction: column;

  width: 100vw;

  height: auto;
  top: 0px;
  left: 0px;
  font-family: "Lato", sans-serif;
}

.pageHeading {

  color: black;
  background-color: white;
  padding: 1em;
  padding-left: 1.8em;
  margin-top: 1em;
  border: none;
  letter-spacing: 1em;
  border: solid black 2px;
  border-radius: 0.2em;
  font-weight: 600;
  font-size: 18px;

}
.projectContainer {
    position: relative;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  width: 100vw;

  margin-top: 1em;
  border-radius: 0.3em;
  background-color: white;

}
.project {

  width: 25vw;
  text-align: center;
  align-self: center;
  height: 40vh;
  border-radius: 0.3em;
  color: white;
  padding: 3em 4em;
}

.overlayOne {
  position: absolute;
  top: 0px;
  left: 0px;
  height: 40vh;
  width: 25%;
  background-color: rgba(255, 181, 33, 0.8);
  z-index: 0;
}

.overlayTwo {
  position: absolute;
  top: 0px;
  left: 25vw;
  height: 40vh;
  width: 25%;
  background-color: rgba(15, 155, 255, 0.8);
  z-index: 0;
}
.overlayThree {
  position: absolute;
  top: 0px;
  left: 50vw;
  height: 40vh;
  width: 25%;
  background-color: rgba(255, 181, 33, 0.8);
  z-index: 0;
}
.overlayFour {
  position: absolute;
  top: 0px;
  left: 75vw;
  height: 40vh;
  width: 25%;
  background-color: rgba(15, 155, 255, 0.8);
  z-index: 0;
}
.front {
  z-index: 1;
}
.pulseElement {
    animation: pulse 11s ease-in-out infinite;
}
.pulseElement12 {
    animation: pulse 12s ease-in-out infinite;
}
.pulseElement14 {
    animation: pulse 13s ease-in-out infinite;
}
.pulseElement16 {
    animation: pulse 14s ease-in-out infinite;
}

@keyframes pulse {
	0% {
    background-color: rgba(255, 181, 33, 0.8);


	}
	50% {
    background-color: rgba(15, 155, 255, 0.8);
	}
  100% {
    background-color: rgba(255, 181, 33, 0.8);
  }
}

</style>
