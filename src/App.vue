<template>
  <div id="app">
    
      <b-navbar sticky toggleable="lg" variant="light" type="light">
        <b-navbar-brand href="#"
          ><img src="./assets/logo.png" width="50px" height="50px" alt="Kitten"
        /></b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="https://drive.google.com/file/d/1LM8v1q6GCDPdRdNBsbDzM15oNd2Ss1dJ/view?usp=sharing">Resume</b-nav-item>
            <b-nav-item href="#projects">Projects</b-nav-item>
            <b-nav-item href="#fun">Fun</b-nav-item>
            <b-nav-item href="#contact">Contact</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
  

    <b-container class="container-fluid mt-5 overflow-hidden">
      <b-row>
        <b-col class="name mb-3"
          >Hi! Yes, you've reached Niharika!<br />
          <span class="desc">
            A high-spirited and joyful <span style="color: #00c2cb">Developer </span>with a deep interest in
            <span style="color: #00c2cb">User Experience</span> working with a
            leading bank based out of
            <span style="color: #00c2cb">Netherlands</span>.</span>
        </b-col>
        <b-col>
          <b-img rounded :src="require('./assets/profile.jpg')" width="450px" height="430px"> </b-img>
        </b-col>
      </b-row>
    </b-container>

    <br /><br /><br />
    <div class="work">
      <br />

       <b-container id="projects">
        <b-row class="text-center d-inline-flex mb-5 mt-4">  
          <b-col ><AccessManagement></AccessManagement></b-col>
          <b-col ><AccessContract></AccessContract></b-col>
        </b-row>
          
     <b-row class="text-center d-inline-flex">
        <b-col> <Mirus></Mirus></b-col>
        <b-col> <OSS></OSS></b-col>
       </b-row>
     </b-container>
      <br /><br />
    </div>
    
    
    
    <br id="fun"/><br />
    <h1  style="font-family: 'Montserrat-Light'">FUN</h1>
    <div class="mt-5 ml-4 cards">
     <Photography></Photography>
     <Designs></Designs>
    </div>  
       <div id="contact" class="work mb-4 mt-5" style="height:300px;backgroundColor:#212529" >
         <br><br><br>
         <p class="desc" style="font-size:25px; color:white;">
           WOULD YOU LIKE TO <span style="color:#F7E06C">CONNECT</span>?
        </p>
        <p class="desc text-muted">
          I'd love that too!
        </p>
        <p class="desc" style="font-size:15px;color:#9CA9B6;">
          Reach me over<br>
          niharika.sharma07@outlook.com<br>
          +91 9962849935
        </p>
       
       </div>
        <div class="h2 mb-3">
    <b-icon icon="linkedin" variant="dark" cursor="pointer" v-on:click="openPage('linkedin')"></b-icon>
     <b-icon icon="facebook" variant="dark" cursor="pointer" class="ml-3 mr-3" v-on:click="openPage('facebook')"></b-icon>
    <b-icon icon="instagram" variant="dark" cursor="pointer" v-on:click="openPage('instagram')"></b-icon>
  </div>
   <p style="font-size:15px;font-family:'Montserrat-Regular';">
        <i> Designed and developed with <b-icon icon="heart-fill" variant="dark"></b-icon> and lots of it by Niharika.</i>
        </p>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import 'bootstrap-vue/dist/bootstrap-vue-icons.min.css'

import AccessManagement from "./components/AccessManagement.vue";
import AccessContract from "./components/AccessContract.vue";
import Mirus from "./components/Mirus.vue";
import OSS from "./components/OSS.vue";
import Photography from "./components/Photography.vue";
import Designs from "./components/Designs.vue";
export default {
  components: { AccessManagement, AccessContract, Mirus, OSS, Photography, Designs },
  methods: {
    openPage(app) {
      if(app=='linkedin'){
        window.location.href = "https://www.linkedin.com/in/niharika-sharma-0b5822b6/";
      }
      else if(app=='facebook'){
        window.location.href = "https://www.facebook.com/niharika.sharma.5095";
      }
      else{
         window.location.href = "https://www.instagram.com/niharikasharma07/";
      }
    },
  },
 
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.work {
  background: #f8f9fa;
}

.name {
  font-family: "Oswald";
  font-size: 30px;
  text-align: left;
}
.desc {
  font-family: "Montserrat-Light";
  font-size: 25px;
}
.cards {
  display: flex;
  justify-content: center;
}
.workshop {
  cursor: pointer;
}
@font-face {
  font-family: "Montserrat-Light";
  src: local("Montserrat-Light"),
    url(./assets/fonts/Montserrat-Light.ttf) format("truetype");
}
@font-face {
  font-family: "Montserrat-Regular";
  src: local("Montserrat-Regular"),
    url(./assets/fonts/Montserrat-Regular.ttf) format("truetype");
}
@font-face {
  font-family: "Oswald";
  src: local("Oswald"),
    url(./assets/fonts/Oswald-Bold.ttf) format("truetype");
}
@font-face {
  font-family: "Voga-Medium";
  src: local("Voga-Medium"),
    url(./assets/fonts/Voga-Medium.otf) format("truetype");
}
</style>
