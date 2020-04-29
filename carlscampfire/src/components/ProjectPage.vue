<template lang="html">
  <div class="pageContainer pulseElement2">
    <h2 class="pageHeading" id="projects">
      PROJECTS
    </h2>

    <div class="projectContainer">
      <a href="https://github.com/Carl-J-M/js_group_0" class="noStyle">
        <div class="project bg1">
          <div class="overlayOne pulseElement"/>
           <h4 class="front center">Cryptic</h4>
           <p class="front">Highly stylized Vue.js puzzle app with custom API & Leaflet.js map integration.</p>
        </div>
      </a>
      <a href="https://github.com/Carl-J-M/reddit_proj" class="noStyle">
        <div class="project front">
          <div class="overlayTwo pulseElement"/>
           <h4 class="front center">Reddit 2.0</h4>
           <p class="front">Vue.js app utilising the reddit API to retrieve posts from a typed subreddit, content reload without page refresh.</p>
        </div>
      </a>
      <a href="https://github.com/Carl-J-M/travel_bucket" class="noStyle">
        <div class="project front">
            <div class="overlayThree"/>
           <h4 class="front center">TravelBucket</h4>
           <p class="front">Ruby/Sinatra application using restful routes to retrieve data from a postgres SQL database. Travel bucket list application with CRUD functionality.</p>
        </div>
      </a>
      <a href="https://lifetaxon.herokuapp.com/" class="noStyle">
        <div class="project front">
                <div class="overlayFour"/>
           <h4 class="front center">Tree of Life</h4>
           <p>The taxonomy of life mapped onto a tree-graph using React.js, API data from gbif.com & react-tree-graph library. Tree graph is mapped from data in state for live reload, state updated on click of tree-graph node.</p>
        </div>
      </a>
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
  top: 0px;
  left: 0px;
  width: 100vw;
  min-height: 40vh;
  height: auto;
  margin-top: 1em;


  background-color: rgba(15, 155, 255, 0.9);
  font-family: "Josefin Sans", sans-serif;
}

.pageHeading {

  color: white;
  padding-left: 1.8em;
  margin-top: 2em;
  margin-bottom: 1em;
  text-align: center;
  min-width: 100%;
  letter-spacing: 0.5em;
  font-weight: 600;
  font-size: 2.5em;
  min-height: 2em;


}
.projectContainer {
  position: relative;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;

  margin-bottom: 10em;
  border-radius: 0.3em;
}

.splashText {
  letter-spacing: 0.2em;
  text-align: center;
  font-size: 2em;
  margin-bottom: 1em;
  font-family: "Josefin Sans", sans-serif;
  color: white;
}

.project {
  position: relative;
  width: 38vw;
  text-align: center;
  align-self: center;
  height: 38vh;
  color: white;
  line-height: 2em;
  font-size: 1em;
  padding: 2em 4em;
  display: block;
  overflow: hidden;
  font-family: "Josefin Sans", sans-serif;

}

.overlayOne {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  background-image: url('../assets/whiteblackwall.jpg');
  background-size: 100% 100%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
  cursor: pointer;
  margin: 0;
}
.overlayOne:hover {

    opacity: 0;
    background-size: 200% 200%;


}
.overlayTwo {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  background-image: url('../assets/redditalien.png');
  background-size: 20%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
}
.overlayTwo:hover {
  opacity: 0;

}
.overlayThree {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  background-image: url('../assets/beachtent.jpg');
  background-size: 105% 100%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
}
.overlayThree:hover {
  opacity: 0;
  background-size: 150% 150%;
}
.overlayFour {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  background-image: url('../assets/colorwheel.jpg');
  background-size: 150% 150%;
  z-index: 0;
  opacity: 1;
  transition-duration: 0.5s;
}
.overlayFour:hover {
  opacity: 0;
  background-size: 100% 100%;
}
.front {
  z-index: 5;
}
.pulseElement {
    animation: pulse 11s ease-in-out infinite;
}
.pulseElement2 {
      animation: pulse2 10s ease-in-out forwards;
}
.center {
  text-align: center;
}
.contactButton {
  color: white;
  cursor: pointer;
  padding: 1em;
  padding-left: 1.8em;
  margin-top: 1em;
  margin-bottom: 4em;
  border: none;
  background-color: transparent;
  letter-spacing: 1em;
  border: solid white 2px;
  border-radius: 0.2em;
  font-weight: 600;
  font-size: 18px;
  font-family: "Josefin Sans", sans-serif;
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
@keyframes pulse2 {
	0% {
    background-color: rgba(255, 181, 33,0.8);
	}
	25% {
    background-color: rgba(255, 181, 33, 0.8);
	}
	100% {
    background-color: rgba(15, 155, 255, 0.8);
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

@media only screen and (max-width: 1200px) {
  .pageHeading {
    font-size: 1em;
    padding-bottom: 0em;
    margin-bottom: 0em;
  }
  .project {

    margin: 0px;
    padding: 1em;
    font-size: 0.8em;
  }
  .projectContainer {
   padding-top: 0px;
  }

  @keyframes slide {

  }
  @keyframes slide2 {

  }

  .splashText {
    padding: 0em 2em;
    color: white;
  }
}

</style>
