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
        <h1>Skills</h1>
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
        <h1>Technical Education</h1>
        <h2>Trainee Software Developer - CodeClan</h2>
        <p>CodeClan is an intensive 16-week Professional Software Development course following agile principles. A full-stack curriculum involing 800+ hours of structured programming.</p>
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
  background: #F7971E;  /* fallback for old browsers */
background: -webkit-linear-gradient(to top, #FFD200, #F7971E);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to top, #FFD200, #F7971E); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

}

.header {

  background-image: url('../assets/about-header-castle.jpg');
  top: 0px;
  left: 0px;
  width: 100vw;
  height: 30vh;
  filter: hue-rotate(3deg);


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


}
.avatar-text {
  position: absolute;
  text-align: left;
  color: #F7971E;
  margin-left: 20%;
  bottom: 10%;
}
.location {
  color: black;

}

.textContainer {
  display: flex;
align-content: flex-start, space-around;

  width: 80%;
  margin: auto;
  height: 70vh;

}

.subContainer {
 width: 45%;
 margin: 20px;

 text-align: left;
 margin-top: 2em;
}

.skillsList {
  list-style-type: none;
  text-align: left;
}
</style>
