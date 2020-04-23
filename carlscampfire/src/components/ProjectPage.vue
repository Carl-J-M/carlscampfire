<template lang="html">
  <div class="pageContainer">
    <h2 class="pageHeading" id="projects">
      <span class="leftSign"></span>
      <span class="leftSign">+</span>
      <span class="leftSign"></span>
      PROJECTS
      <span class="rightSign"></span>
      <span class="rightSign">-</span>
      <span class="rightSign"></span>
    </h2>

    <div class="projectContainer">

      <div class="project bg1">
        <div class="overlayOne pulseElement"/>
         <h4 class="front center">Cryptic</h4>
         <p class="front">Puzzle app with admin login and secret event location map.</p>
      </div>

      <div class="project front">
        <div class="overlayTwo pulseElement12"/>
         <h4 class="front center">Reddit 2.0</h4>
         <p class="front">Vue.js app utilising the reddit API to retrieve posts from a typed subreddit, no page refresh.</p>
      </div>
      <div class="project front">
          <div class="overlayThree pulseElement14"/>
         <h4 class="front center">TravelBucket</h4>
         <p class="front">Ruby/Sinatra application using restful routes to retrieve data from a postgres SQL database. Travel bucket list application with CRUD functionality.</p>
      </div>
      <div class="project front">
              <div class="overlayFour pulseElement16"/>
         <h4 class="front center">Randomflix</h4>
         <p class="front">A simple film randomizer to help break the stalemate with my flatmates about what movie to watch.</p>
      </div>
    </div>
    <div class="splashText">
      I'm actively seeking my first Junior Developer position.
    </div>

    <a href="#contact" class="noStyle"><button class="contactButton">
      CONTACT
    </button></a>


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
  min-height: 40vh;
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

  margin-bottom: 1em;
  text-align: center;
  min-width: 100%;
  letter-spacing: 1em;
  color: black;
  font-weight: 600;
  font-size: 1.5em;
  min-height: 8em;


}
.projectContainer {
  position: relative;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  width: 100vw;


  margin-bottom: 10em;
  border-radius: 0.3em;
  background-color: white;

}
.splashText {
  font-size: 1.5em;
  margin-bottom: 1em;
}
.project {

  width: 25vw;
  text-align: left;
  align-self: center;
  height: 40vh;
  border-radius: 0.3em;
  color: black;

  font-size: 1.4em;
  padding: 1em;
  display: block;
  overflow: hidden;

}

.overlayOne {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 25%;
  height: 100%;
  background-image: url('../assets/whiteblackwall.jpg');
  background-size: 100% 100%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
  cursor: pointer;
}
.overlayOne:hover {

    opacity: 0;
    background-size: 200% 200%;


}
.overlayTwo:hover {
  opacity: 0;

}
.overlayThree:hover {
  opacity: 0;
  background-size: 150% 150%;
}
.overlayFour:hover {
  opacity: 0;
  background-size: 100% 100%;
}

.overlayTwo {
  position: absolute;
  top: 0px;
  left: 25vw;
  height: 40vh;
  width: 25%;
  cursor: pointer;
  background-image: url('../assets/redditalien.png');
  background-size: 20%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
}
.overlayThree {
  position: absolute;
  top: 0px;
  left: 50vw;
  height: 40vh;
  width: 25%;
  cursor: pointer;
  background-image: url('../assets/beachtent.jpg');
  background-size: 200% 200%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
}
.overlayFour {
  position: absolute;
  top: 0px;
  left: 75vw;
  height: 40vh;
  width: 25%;
  cursor: pointer;
  background-image: url('../assets/colorwheel.jpg');
  background-size: 200% 200%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
}
.front {
  z-index: 5;
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
.bg1 {
  /* background-image: url('../assets/reddark.jpg'); */
  background-color: white;
}
.center {
  text-align: center;
}
.leftSign {

  animation: slide 7s ease-in-out infinite;
  overflow: hidden;
  color: green;
}
.rightSign {
  animation: slide2 4s ease-in-out infinite;
  overflow: hidden;
  color: red;
}
.contactButton {
  color: black;
 cursor: pointer;
  padding: 1em;
  padding-left: 1.8em;
  margin-top: 1em;
  margin-bottom: 4em;
  border: none;
  background-color: transparent;
  letter-spacing: 1em;
  border: solid black 2px;
  border-radius: 0.2em;
  font-weight: 600;
  font-size: 18px;
}
.noStyle {
  text-decoration: none;
}
@keyframes pulse {
	0% {
    background-color: rgba(255, 181, 33);


	}
	20% {
    background-color: rgba(15, 155, 255);
	}
  100% {
    background-color: rgba(255, 181, 33);
  }
}
@keyframes slide {
  0%{
      margin-right: 1em;
      font-size: 0.5em;
  }
  20%{
    margin-right: -0.1em;
    font-size: 4em;
  }
  80%{
    margin-right: -0.1em;
    font-size: 4em;
  }
  100%{
    margin-right: 1em;
    font-size: 0.5em;
  }
}
@keyframes slide2 {
  0%{
      margin-left: 0.1em;
      font-size: 1em;
  }

  50%{
    margin-left: 1em;
    font-size: 4em;
  }

  100%{
    margin-left: 0.1em;
    font-size: 1em;
  }
}

</style>
