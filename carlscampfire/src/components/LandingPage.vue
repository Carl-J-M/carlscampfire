<template lang="html">
  <div class="pageContainer">
    <div class="splashText front">
      <h1>Carl Mensah</h1>
      <h2>SOFTWARE DEVELOPER</h2>
      <a href="#projects">
        <button class="viewWorkButton front">VIEW WORK</button>
      </a>
    </div>
    <div class="overlay pulseElement"/>
      <div class="vimeo-wrapper">
         <iframe
         src="https://player.vimeo.com/video/326324986?background=1&autoplay=1&loop=1&byline=0&title=0"
        frameborder="0"
        webkitallowfullscreen
        mozallowfullscreen
        allowfullscreen>
        </iframe>
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

  z-index: -5;
}

.splashText {
  justify-content: center;
  align-self: center;
  text-align: center;
  margin: auto;
  margin-top: 50vh;
  color: white;
  font-family: "Josefin Sans", sans-serif;
}

.viewWorkButton {
  color: white;
  background-color: transparent;
  cursor: pointer;
  border: solid white 2px;
  border-radius: 0.2em;

  padding: 1em;
  padding-left: 1.8em;
  margin-top: 1em;

  font-weight: 600;
  font-size: 1em;
  font-family: "Josefin Sans", sans-serif;
  letter-spacing: 1em;
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
   height: 56.25vw;
   min-height: 100vh;
   min-width: 177.77vh;
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
