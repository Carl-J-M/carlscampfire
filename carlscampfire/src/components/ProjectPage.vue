<template lang="html">
  <div class="pageContainer">
    <div class="overlay"/>
    <h1 class="pageHeading" id="projects">
      PROJECTS
    </h1>
    <div class="parent">
      <div class="card1 card" v-on:click="selectProject($event, 0)"></div>
      <div class="card2 card" v-on:click="selectProject($event, 1)"></div>
      <div class="card3 card" v-on:click="selectProject($event, 2)"></div>
      <div class="card1text cardtext">{{ projects[0].title}}
        <p  class="lifetaxon"><a href="https://lifetaxon.herokuapp.com/">View On Heroku</a></p>
        </div>
      <div class="card2text cardtext">{{ projects[1].title}}</div>
      <div class="card3text cardtext">{{ projects[2].title}}</div>
    </div>
            <h2 class="displayHeading">{{selectedProjectTitle}}<a :href="selectedProjectLink"><div class="icon github hidden"></div></a></h2>
        <p class="displayText">{{selectedProjectDescription}}</p>
    <div class="displayContainer">
        <div class="tag" v-for="tag in selectedProjectTags">
          <div>{{tag}}</div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedProjectTitle: "Click on a project above to find out more.",
      selectedProjectDescription: "",
      selectedProjectTags: [],
      selectedProjectLink: "#contact",
      projects: 
      [
        {
          title: "LIFETAXON",
          description: "An interactive map of the taxonomy of life, using live data from gbif.com containing over 240,000 datapoints. Fetch requests are constructed using the API key to make new requests and update the tree with live data. Data is formatted for use with react-tree-graph and passed into state. Exercise in state management and using state to present data fluidly.",
          tags: ["React","react-tree-graph","JavaScript","HTML5","CSS3","API Data","Data Visualization", "Dynamic Queries", "Data Formatting", "State Manipulation"],
          link: "https://github.com/Carl-J-M/TreeOfLife"
        },
              {
          title: "CRYPTIC",
          description: "An application designed to generate hype as an internet mystery. I designed and built a fake 'redacted document' using HTML, CSS & Vue which takes data from a custom API my teammates built, allowing for dynamic riddles to be dropped into our fake document.",
          tags: ["Vue.js", "HTML5", "CSS3", "Leaflet.js", "MongoDB", "Custom Backend", "Login", "Express","Trello"],
          link: "https://github.com/Carl-J-M/js_group_0"
        },
        {
          title: "TRAVELBUCKET",
          description: "Ruby/Sinatra travel bucket list application, using restful routes & a postgres database.",
          tags: ["Ruby", "Sinatra", "HTML5", "CSS3", "SQL", "POSTGRES", "RDBMS", "Relationships", "OOP", "Restful Routes"],
          link: "https://github.com/Carl-J-M/travel_bucket"
        }
      ]
    }
  },
  methods: {
    selectProject: function (event, id) {
      console.log(id);

      
      this.selectedProjectTitle = this.projects[id].title;
      this.selectedProjectDescription = this.projects[id].description;
      this.selectedProjectTags = this.projects[id].tags;
      this.selectedProjectLink = this.projects[id].link;
      return;

  }

}
}
</script>

<style lang="css" scoped>

.pageContainer {
  font-family: "Josefin Sans", sans-serif;
  position: relative;
  top: 0px;
  left: 0px;
  min-width: 100vw;
  min-height: 100vh;
  background-color: white;
  z-index: 0;
}
.pageHeading {
  text-align: center;
  width: 100%;
  padding-top: 2em;
  padding-bottom: 2em;
  letter-spacing: .5em;
  color: white;
  background-color: rgba(15, 155, 255, 0.9);
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); 
}
.overlay {

  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  background-color: black;
  clip-path: rect(10px, 190px, 190px, 10px);

}
.parent {
display: grid;
grid-template-columns: .1fr repeat(3, 1fr) .1fr;
grid-template-rows: .5fr 4fr repeat(3, 1fr);
grid-column-gap: 0px;
grid-row-gap: 0px;
padding: 0.1em;

}

.card {
  text-align: center;
  height: auto;
  min-height: 15em;
  margin: 0em 1em;
  transition: all ease-in-out 0.4s;
  /* box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); */
}
.card:hover {
  cursor: pointer;
  background-size: 250% 250%;
}

.cardtext {
  text-align: center;
  height: auto;
  margin: 0em 1em;
  padding: 1em;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); 
    z-index: 0;
  color: black;
}

.card1 { grid-area: 2 / 2 / 3 / 3; 
background-size: 100% 100%;
background-image: url('../assets/lifetaxon.png');
background-repeat: no-repeat;

}
.card2 { grid-area: 2 / 3 / 3 / 4;
background-size: 100% 100%;
background-image: url('../assets/cryptic.png');
background-repeat: no-repeat;

}
.card3 { grid-area: 2 / 4 / 3 / 5; 
background-size: 100% 100%;
background-image: url('../assets/travelbucket.png');
background-repeat: no-repeat;

}
.card1text { grid-area: 3 / 2 / 4 / 3;

}
.card2text { grid-area: 3 / 3 / 4 / 4; 

}
.card3text { grid-area: 3 / 4 / 4 / 5;

 }

.displayContainer {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding-bottom: 5em;
  margin: 0 auto;
  width: 80%;


}

.displayHeading {
  text-align: center;
  color: black;
  width: 100vw;
  font-size: 2em;

}

.displayText {
  text-align: center;
  padding: 1em 2em;
  font-size: 1em;
  line-height: 1.2em;
  width: 80%;
  margin: 0 auto;
  margin-top: 1em;
    /* box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);  */
}

.tagContainer {
  display: flex;
  flex-flow: column wrap;
  height: 100%;
}
.tag {
  padding: 0.4em;
  margin: 0em 0.5em;
  margin-top: 2em;
  /* border-radius: 0.5em; */
  text-align: center;
  color: dodgerblue;
  font-size: 2em;
  font-weight: 800;
  width: auto;
  height: 40%;

    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.2), 0 6px 10px 0 rgba(0, 0, 0, 0.01); 
  
}
.github {
  height: 2em;
  width: 2em;
  padding: 1em;

  margin: 0 auto;
  margin-top: 1em;
  background-image: url('../assets/github.svg');
  background-size: 100% 100%;
  
}

.lifetaxon {
  color: dodgerblue;

}
.lifetaxon a {
  text-decoration: none;
}
</style>
