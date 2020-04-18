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
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        <ul>
          <li>1</li>
          <li>2</li>
          <li>3</li>
          <li>4</li>
          <li>5</li>
        </ul>
    </div>
    <div class="subContainer">
        <h1>Technical Education</h1>
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

 text-align: center;
 margin-top: 2em;
}
</style>
