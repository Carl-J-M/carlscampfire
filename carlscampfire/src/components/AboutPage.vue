<template lang="html">
<div class="pageContainer" id="contact">
  <div class="header">
    <a href="https://github.com/Carl-J-M"><div class="icon github"></div></a>
    <a href="https://www.linkedin.com/in/carl-mensah-aa27661a7/"><div class="icon linkedin"></div></a>
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
        <h3 class="subheading">BACKGROUND</h3>
        <h4 class="left subheading">Where?</h4>
        <p class="left subtext">
        I grew up near Stoke-On-Trent in the midlands.
        I worked as a cocktail bartender at Dishoom in Edinburgh before I decided to join CodeClan.</p>
        <h4 class="left subheading">Why?</h4>
        <p class="left subtext">
          I decided to leave the hospitality industry after feeling as though my ability to learn new things began to stagnate. I didn't feel challenged or excited by my work and resolved to learn all I could about computer programming and software development.
        </p>
        <h4 class="left subheading">How?</h4>
                <p class="left subtext">I spent several years studying software development as a hobby while working in my previous industry.</p>
                <p class="left subtext">I decided to enroll at CodeClan in January 2020 and become a professional software developer.</p>
    </div>
    <div class="subContainer pulseElement">
        <h3 class="subheading">EDUCATION</h3>
        <h4 class="left subheading">CodeClan, Edinburgh</h4>
        <p class="left subtext">An intensive 16-week Professional Software Development course following agile principles. A full-stack curriculum involing 800+ hours of structured programming.
        <p class="left subtext">Throughout the course I gained valuable experience using a wide variety of technologies, both in group settings and individually.</p>
        <h4 class="left subheading">Self Study</h4>

        <p class="left subtext">
        I love learning about new technologies, problem solving techniques and UI/UX design.
        </p>
        <p class="left subtext">
        I'm eager to work with more experienced developers I can learn from and improve my skills.
        </p>
        <p class="left subtext">
        While I'm most excited to improve my front-end skills, I have a solid grasp of back-end fundamentals and would be eager to learn more on the journey to Full Stack.
        </p>
</p>
    </div>
    <div class="subContainer pulseElement">
      <h3 class="subheading">SKILLS</h3>
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
  font-family: 'Josefin Sans', sans-serif;
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
  font-family: "Josefin Sans", sans-serif;
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
 margin-bottom: 4em;

 margin-top: -1em;
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
  clip-path: polygon(0 0, 62% 0, 62% 100%, 0% 100%);

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
.left {
  text-align: left;
}
.subheading {
  margin-top: 1em;
  margin-bottom: 0.5em;
}
.subtext {
  font-size: 1em;
  margin-bottom: 0.5em;
  line-height: 1.2em;
}
@keyframes pulse {
	0% {
    background-color: rgba(255, 181, 33,0.9);
	}
	25% {
    background-color: rgba(255, 181, 33, 0.9);
	}
	100% {
    background-color: rgba(15, 155, 255, 0.9);
	}
}

@media only screen and (max-width: 1200px) {
  .textContainer {
     flex-direction: row;

  }
  .subContainer {
    width: 100%;
    margin: 0.2em;
    margin-top: 1.5em;
    padding: 1em;
    margin-bottom: 2.5em;
  }
  .avatar {
    right: 20px;
  }
  .avatar-text {
    margin-left: 5vw;
    text-align: left;
    font-size: 0.8em;
  }
  .header {
    background-image: none;
    background-color: white;
    max-height: 10em;
  }
  .github {
    margin-left: 5vw;
  }
  .linkedin {
    margin-left: 20vw;
  }
  .avatar {
    height: 8em;
    width: 10em;
  }
  .skill {
    width: 20%;
  }
}
</style>
