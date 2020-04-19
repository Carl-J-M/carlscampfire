<template lang="html">
  <div class="pageContainer">
    <div class="splashText">
      <h1>Carl Mensah</h1>
      <h2>SOFTWARE DEVELOPER</h2>
      <button class="viewWorkButton">VIEW WORK</button>
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


  background: linear-gradient(90deg, #00d2ff 0%, #3a47d5 100%);

}

.splashText {
  justify-content: center;
  align-self: center;
  margin: auto;
  color: white;
  text-align: center;
  font-family: "Roboto", sans-serif;
}

.viewWorkButton {
  color: white;

  padding: 1em;
  padding-left: 1.8em;
  margin-top: 1em;
  border: none;
  background-color: transparent;
  letter-spacing: 1em;
  border: solid white 2px;
  border-radius: 0.2em;
  font-weight: 600;
  font-size: 18px;
}
.viewWorkButton:hover {
  background-color: dodgerblue;
  color: white;
}

</style>
