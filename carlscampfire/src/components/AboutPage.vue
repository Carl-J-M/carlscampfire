<template lang="html">
<div class="pageContainer">
  <div class="header">
    <div class="icon github"></div>
    <div class="icon linkedin"></div>
      <div class="avatar front"/>

      <div class="avatar-text front">
        <h3 class="location">Edinburgh, Scotland</h3>
        <h3>carlmensahmail@gmail.com</h3>
        <h3>07493 011 396</h3>
      </div>

      <div class="overlay pulseElement"/>
  </div>
  <div class="textContainer">
    <div class="subContainer pulseElement">
        <h3>TECHNICAL EDUCATION</h3>
    </div>
    <div class="subContainer pulseElement">
        <h3>BACKGROUND</h3>
    </div>
    <div class="subContainer pulseElement">
      <h3>SKILLS</h3>
       <div class="skillsContainer">
         <div class="skill">
           <h3 class="skillHeading">JavaScript</h3>
           <i class="fab fa-js"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">HTML5</h3>
           <i class="fab fa-html5"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">CSS3</h3>
           <i class="fab fa-css3-alt"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">Node.js</h3>
           <i class="fab fa-node-js"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">SQL</h3>
           <i class="fas fa-database"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">Express</h3>
           <i class="fas fa-server"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">Ruby</h3>
           <i class="far fa-gem"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">React</h3>
           <i class="fab fa-react"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">Vue.js</h3>
           <i class="fab fa-vuejs"></i>
         </div>
         <div class="skill">
           <h3 class="skillHeading">Sass</h3>
           <i class="fab fa-sass"></i>
         </div>


         </div>

       </div>
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
  flex-direction: column;
  width: 100vw;
  height: auto;
  top: 0px;
  left: 0px;
  /* background-image: url('../assets/lakepier.jpg'); */
  /* background-image: url('../assets/caltonhill.jpg'); */
  background-size: 100%;

  /* background-image: url('../assets/bricksivy.jpg'); */

}

.header {
  top: 0px;
  left: 0px;
  width: 100vw;
  height: 25vh;
  min-height: 10em;
  filter: hue-rotate(0deg);
  -webkit-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  background-image: url('../assets/about-header-castle.jpg');
  background-size: 100%;
}

.avatar {
  position: absolute;
  bottom: 0px;
  margin-left: 17vw;
  background-image: url('../assets/carl-avatar.png');
  background-repeat: no-repeat;
  min-height: 10em;
  height: auto;
  width: 10em;
  background-size: 100% 100%;
}
.avatar-text {
  position: absolute;
  text-align: right;
  font-family: 'Lato', sans-serif;
  color: white;
  margin-left: 40vw;
  bottom: 50%;
}
.location {
  color: black;
}
.textContainer {
  display: flex;
  align-content: flex-start, space-around;
  flex-wrap: wrap;
  font-family: "Roboto", sans-serif;
  width: 80%;
  margin: auto;
  margin-top: 0px;
  height: 100%;

}

.subContainer {
 width: 30%;
 height: auto;
 margin: 0em 1em;
 padding: 2em;
 color: white;
 font-size: auto;
 text-align: center;
 border-radius: 0.2em;

}

.skillsList {

  list-style-type: none;
  text-align: left;
}
.overlay {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;

  z-index: -1;
  /* clip-path: polygon(0 0, 100% 0%, 90% 100%, 10% 100%); */
  clip-path: polygon(0 0, 62% 0, 62% 100%, 0% 100%);

  /* clip-path: polygon(0 0, 100% 0, 80% 0%, 50% 52%, 100% 1000%, 100% 100%, 0 100%); */
}
.front {
  z-index: 2;
}
.pulseElement {
    animation: pulse 10s ease-in-out forwards;
}
.icon {
  width: 2.5em;
  height: 2.5em;

}

.github {
  position: absolute;
  background-image: url('../assets/github.svg');
  background-size: 100% 100%;
  margin-left: 45vw;
  bottom: 1em;

}
.linkedin {
  position: absolute;
  background-image: url('../assets/linkedin.png');
  background-size: 100% 100%;
  margin-left: 50vw;
  bottom: 1em;
}
.skillsContainer {
  display: flex;
  flex-wrap: wrap;
  margin: 0px;
  margin-top: 0.5em;
  padding: 0px;
  font-size:  3em;
}
.skill {
  width: 50%;
  padding-bottom: 0.5em;

}
.skillHeading {
  font-size: 0.3em;
}
@keyframes pulse {
	0% {
    background-color: rgba(255, 181, 33,0.2);


	}
	25% {
    background-color: rgba(255, 181, 33, 0.8);


	}
	100% {
    background-color: rgba(15, 155, 255, 0.8);
	}
}
</style>
