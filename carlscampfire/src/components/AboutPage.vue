<template lang="html">
<div class="pageContainer">
  <div class="header">
      <div class="avatar front"/>
      <div class="avatar-text front">
        <h3 class="location">Edinburgh, Scotland</h3>
        <h3>carlmensahmail@gmail.com</h3>
        <h3>07493 011 396</h3>
      </div>
      <div class="overlay"/>
  </div>
  <div class="textContainer">
    <div class="subContainer">
        <h3>SKILLS</h3>
        <p>I've used a wide variety of different technologies and languages to tackle a range of different problems in the past. Here's a few of those:</p>
        <ul class="skillsList">
          <li>HTML</li>
          <li>CSS</li>
          <li>JavaScript</li>
          <li>Vue.js | React</li>
          <li>Java</li>
          <li>SQL</li>
          <li>Ruby</li>
          <li>Express</li>
          <li>MongoDB</li>
        </ul>
    </div>
    <div class="subContainer">
        <h3>TECHNICAL EDUCATION</h3>
        <p>CodeClan is an intensive 16-week Professional Software Development course following agile principles. A full-stack curriculum involing 800+ hours of structured programming.</p>
    </div>
    <div class="subContainer">
        <h3>BACKGROUND</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
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
  height: 100vh;
  top: 0px;
  left: 0px;
  background-image: url('../assets/lakepier.jpg');




}

.header {


  top: 0px;
  left: 0px;
  width: 100vw;
  height: 25vh;
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
  margin-left: 35%;
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
  right: 30%;

  bottom: 30%;
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
  height: auto;
  background-color:  rgba(15, 155, 255, 0.9);



}

.subContainer {
 width: 30%;
 height: auto;
 margin: 1em 1em;
 padding: 2em;
 color: white;
 font-size: 1em;
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
  background-color: rgba(15, 155, 255, 0.9);
  z-index: 0;
  clip-path: polygon(0 0, 100% 0%, 90% 100%, 10% 100%);


  /* clip-path: polygon(0 0, 100% 0%, 100% 48%, 0 48%); */
}
.front {
  z-index: 2;
}
</style>
