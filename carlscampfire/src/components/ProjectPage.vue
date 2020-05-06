<template lang="html">
  <div class="pageContainer">
    <div class="overlay"/>
    <h1 class="pageHeading" id="projects">
      PROJECTS
    </h1>
    <div class="parent">
      <div class="card1 card" v-on:click="selectProject($event, 0)" href="#projectTitle"></div>
      <div class="card2 card" v-on:click="selectProject($event, 1)"></div>
      <div class="card3 card" v-on:click="selectProject($event, 2)"></div>
      <div class="card1text cardtext">{{ projects[0].title}}
        <p  class="lifetaxon"><a href="https://lifetaxon.herokuapp.com/">View On Heroku</a></p>
        </div>
      <div class="card2text cardtext">{{ projects[1].title}}</div>
      <div class="card3text cardtext">{{ projects[2].title}}</div>
    </div>
            <h2 class="displayHeading" id="projectTitle">
              {{selectedProjectTitle}}
              <a :href="selectedProjectLink">
                <div class="icon github hidden pulseElement"></div>
             </a>
            </h2>
          
        <p class="displayText">{{selectedProjectDescription}}</p>
    <div class="displayContainer">
        <div class="tag" v-for="tag in selectedProjectTags">
          <div>{{tag}}</div>
        </div>
    </div>
    <div class="footer">
      <h4 class="copyright">Carl Mensah © 2020</h4>
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
          description: "An interactive map of the taxonomy of life, using the gbif.com API containing over 240,000 datapoints. Fetch requests are constructed dynamically by using keys extracted from a given record. The data from these new requests updates the state. This state data is passed down as a prop to the tree graph itself. Exercise in state management and using state to present data fluidly.",
          tags: ["React","react-tree-graph","JavaScript","HTML5","CSS3","API Data","Data Visualization", "Dynamic Queries", "Data Formatting", "State Manipulation"],
          link: "https://github.com/Carl-J-M/TreeOfLife"
        },
              {
          title: "CRYPTIC",
          description: "An application designed to generate hype as an internet mystery. I designed and built a fake 'redacted document' using HTML, CSS & Vue.js data properties. The application takes data from a custom API we built as a team, this data populates the document and provides the information to decode the password. A successful password attempt routes the user to a page with a Leaflet.js map and instructions. Admin login allows for creating new events.",
          tags: ["Vue.js", "HTML5", "CSS3", "Leaflet.js", "MongoDB", "Custom Backend", "Login", "Express","Trello","Wireframing"],
          link: "https://github.com/Carl-J-M/js_group_0"
        },
        {
          title: "TRAVELBUCKET",
          description: "A personal travel bucket list application designed for a single user as a place to tick off destinations and write notes about their travels. Full CRUD functionality for Continents, Countries & Cities.",
          tags: ["Ruby", "Sinatra", "HTML5", "CSS3", "SQL", "POSTGRES", "RDBMS", "Relationships", "OOP", "Restful Routes", "CRUD"],
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
    -webkit-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
  box-shadow: 0px 0px 28px -1px rgba(0,0,0,0.75);
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
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
.card:hover {
  cursor: pointer;
  background-size: 120% 120%;
  
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
  padding: 1em;
  margin-top: 0px;

}

.displayText {
  text-align: center;
  padding: 1em 2em;
  font-size: 1em;
  line-height: 1.5em;
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

  font-size: 2em;
  font-weight: 800;
  width: auto;
  height: 40%;

    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.2), 0 6px 10px 0 rgba(0, 0, 0, 0.01); 
  
}
.github {
  height: 2em;
  width: 2em;
  padding: 1.5em;

  margin: 0 auto;
  margin-top: 1em;
  background-image: url('../assets/github.svg');
  background-size: 100% 100%;
  border-radius: 50%;
  transition: all ease-in-out 1s;
}

.lifetaxon {
  color: dodgerblue;

}
.lifetaxon a {
  text-decoration: none;
}
.footer {
  height: auto;
  width: 100%;
  background: #000000;  /* fallback for old browsers */
background: -webkit-linear-gradient(to top, #434343, #000000);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to top, #434343, #000000); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
background-size: 100% 150%;

}
.copyright {
  font-size: 0.7em;
  color: white;
  text-align: center;
  bottom: 1em;
  padding: 2em;
}
.pulseElement {
    animation: pulse 10s ease-in-out infinite;
}
@keyframes pulse {
  0% {
  background-color: rgba(255, 151, 33, 0.5);

	}
	33% {
    background-color: rgb(33, 196, 255);

	}

	66% {
    background-color: rgb(44, 165, 78);

	}

  100% {
  background-color: rgb(255, 151, 33, 0.5);
  }
}
</style>
