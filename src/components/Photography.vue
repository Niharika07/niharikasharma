<template>
  <div id="Photography">
      
      <figure v-b-modal.modalPh class="figure"  @click='showPh=true'>
        <img
          src="../assets/amsterdam.jpg"
          class="figure-img img-fluid z-depth-1"
          style="width: 500px; height: 340px"
        />
        <figcaption class="figure-caption mb-3"  style="font-family: 'Montserrat-Regular';font-size: 20px;color: black;">
          Photography
        </figcaption>
      </figure>


 <b-modal id="modalPh" size="xl" v-model='showPh' >
   <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Photography/ImgOne.jpg')" width="500px" height="350px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgTwo.jpg')" width="500px" height="350px"></b-img>
    </b-col>
  </b-row>
 </b-container>

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Photography/ImgThree.jpg')" width="500px" height="350px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgFour.jpg')" width="500px" height="350px"></b-img>
    </b-col>
  </b-row>
 </b-container>
<b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgFive.jpg')" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
       <b-img rounded :src="require('../assets/Photography/ImgSix.jpg')" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
  </b-container>
  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Photography/ImgSeven.jpg')" width="400px" height="400px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgEight.jpg')" width="400px" height="400px"></b-img>
    </b-col>
  </b-row>
 </b-container>

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Photography/ImgNine.jpg')" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgTen.jpg')" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
 </b-container>

 <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Photography/ImgThirteen.jpg')" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgFourteen.jpg')" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
 </b-container>
 
 <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Photography/ImgEleven.png')" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Photography/ImgTwelve.jpg')" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
 </b-container>
 
  

 <template v-slot:modal-footer>
        <b-button variant='warning' size='md' class='float-right' @click='showPh=false'>Close</b-button>
 </template>
        
 <template #modal-header>
     <div class="w-100">
          <span class="text-center" style="color:#00c2cb;font-family:'Montserrat-Regular'"> <h1> Photography </h1> </span>
          <span class="text-center" style="font-family:'Montserrat-Regular'"><h6> <i>Capturing the world through my lens!</i> </h6> </span>
     </div>
 </template>
 </b-modal> 
      
  
  </div>
</template>

<script>

export default {
    data() {
    return {
      showPh: false,
    };
  },
}
</script>

<style>
  


</style>
