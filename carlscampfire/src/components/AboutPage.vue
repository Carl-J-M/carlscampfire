<template lang="html">
<div class="pageContainer">
  <div class="header">
      <div class="avatar"/>
      <div class="avatar-text">
        <h3 class="location">Edinburgh, Scotland</h3>
        <h3>carlmensahmail@gmail.com</h3>
        <h3>07493 011 396</h3>
      </div>
  </div>
  <div class="textContainer">
    <div class="subContainer">
        <h2>SKILLS</h2>
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
        <h2>TECHNICAL EDUCATION</h2>
        <h3>Trainee Software Developer - CodeClan</h3>
        <p>CodeClan is an intensive 16-week Professional Software Development course following agile principles. A full-stack curriculum involing 800+ hours of structured programming.</p>
    </div>
    <div class="subContainer">
        <h2>BACKGROUND</h2>
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
  background: linear-gradient(180deg, #00d2ff 0%, #3a47d5 100%);

}

.header {

  background-image: url('../assets/about-header-castle.jpg');
  /* background-size: 100% 100%; */
  top: 0px;
  left: 0px;
  width: 100vw;
  height: 30vh;
  filter: hue-rotate(0deg);
  -webkit-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);


}

.avatar {
  position: absolute;

  bottom: 0px;
  margin-left: 5%;
  background-image: url('../assets/carl-avatar.png');
  background-repeat: no-repeat;
  min-height: 10em;
  height: auto;
  width: 10em;
  background-size: 100% 100%;
  filter: grayscale();


}
.avatar-text {
  position: absolute;
  text-align: left;
  font-family: 'Lato', sans-serif;
  font-size: 1.3em;
  color: dodgerblue;
  margin-left: 20%;

  bottom: 10%;
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
  height: 70vh;


}

.subContainer {
 width: 30%;
 margin: 2em 1em;
 padding: 2em;
 color: white;
 text-align: left;
 margin-top: 2em;
}

.skillsList {
  list-style-type: none;
  text-align: left;
}
</style>
