<template lang="html">
  <div class="pageContainer">
    <div class="splashText">
      <h1>Carl Mensah</h1>
      <h2>SOFTWARE DEVELOPER</h2>
      <button class="viewWorkButton">VIEW MY WORK</button>
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
  width: 100vw;
  height: 100vh;
  top: 0px;
  left: 0px;
  flex-direction: column;


  background: #F7971E;  /* fallback for old browsers */
background: -webkit-linear-gradient(to bottom, #FFD200, #F7971E);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to bottom, #FFD200, #F7971E); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}

.splashText {
  justify-content: center;
  align-self: center;
  margin: auto;
  color: black;
  text-align: center;
  font-family: "Roboto", sans-serif;
}

.viewWorkButton {
  color: black;
  background-color: white;

  padding: 0.5em;
  margin-top: 1em;

  border-radius: 1em;

  font-weight: 600;
  font-size: 18px;
}

</style>
