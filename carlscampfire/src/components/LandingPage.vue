<template lang="html">
  <div class="pageContainer">
    <div class="splashText front">
      <h1>Carl Mensah</h1>
      <h2 class="underline">SOFTWARE DEVELOPER</h2>
      <a href="#projects">
        <button class="viewWorkButton front">VIEW WORK</button></a>
    </div>
    <div class="overlay pulseElement"/>
      <div class="vimeo-wrapper">
         <iframe src="https://player.vimeo.com/video/326324986?background=1&autoplay=1&loop=1&byline=0&title=0"
                 frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
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

  /* background-image: url('../assets/campfire.jpg'); */
  background-size: 100% 100%;
z-index: -5;
  /* background: linear-gradient(90deg, #00d2ff 0%, #3a47d5 100%); */

}

.splashText {
  justify-content: center;
  align-self: center;
  margin: auto;
  margin-top: 50vh;
  color: white;
  text-align: center;
  font-family: "Josefin Sans", sans-serif;
}

.viewWorkButton {
  color: white;
 cursor: pointer;
  padding: 1em;
  padding-left: 1.8em;
  margin-top: 1em;
  border: none;
  background-color: transparent;
  letter-spacing: 1em;
  border: solid white 2px;
  border-radius: 0.2em;
  font-weight: 600;
  font-size: 1em;
  font-family: "Josefin Sans", sans-serif;
}
.viewWorkButton:hover {
  background-color: white;
  color: dodgerblue;
}
.overlay {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100vw;
  height: 100vh;
  z-index: 0;
  clip-path: circle(50% at 50% 60%);

  /* clip-path: polygon(0 0, 100% 0%, 100% 48%, 0 48%); */
}
.front {
  z-index: 2;
}
.pulseElement {
    animation: pulse 10s ease-in-out forwards;
}

.vimeo-wrapper {
   position: fixed;
   top: 0;
   left: 0;
   width: 100%;
   height: 100%;
   z-index: -1;
   pointer-events: none;
   overflow: hidden;
}
.vimeo-wrapper iframe {
   width: 100vw;
   height: 56.25vw; /* Given a 16:9 aspect ratio, 9/16*100 = 56.25 */
   min-height: 100vh;
   min-width: 177.77vh; /* Given a 16:9 aspect ratio, 16/9*100 = 177.77 */
   position: absolute;
   top: 50%;
   left: 50%;
   transform: translate(-50%, -50%);
}
@keyframes pulse {
  0% {
    background-color: rgba(255, 181, 33,0.0);

	}
	25% {
    background-color: rgba(255, 181, 33, 0.3);
    clip-path: circle(30% at 50% 60%);

	}
  40% {
    clip-path: circle(100% at 50% 60%);
  }
	100% {
    background-color: rgba(15, 155, 255, 0.3);
    clip-path: circle(100% at 50% 60%);
	}
}
@media only screen and (max-width: 1200px) {
   .pageContainer {
     background-size: 120% 100%;
   }
}
@media only screen and (max-width: 400px) {
   .pageContainer {
     background-size: 300% 100%;
   }
}
</style>
