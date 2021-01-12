<template>
  <div id="Designs">
      
       <figure v-b-modal.modalDg class="figure"  @click='showDg=true'>
        <img
          src="../assets/Designs/thankYou.jpg"
          class="figure-img img-fluid z-depth-1"
          style="width: 480px; height: 340px"
        />
        <figcaption
          class="figure-caption mb-3"
          style="
            font-family: 'Montserrat-Regular';
            font-size: 20px;
            color: black;
          "
        >
          Lettering Designs
        </figcaption>
      </figure>


 <b-modal id="modalDg" size="xl" v-model='showDg' >

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Designs/ImgOne.jpg')" width="500px" height="350px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Designs/ImgTwo.jpg')" width="500px" height="350px"></b-img>
    </b-col>
  </b-row>
 </b-container>
  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded class="mt-2" :src="require('../assets/Designs/ImgThree.jpg')" width="500px" height="480px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Designs/ImgFour.jpg')" width="500px" height="500px"></b-img>
    </b-col>
  </b-row>
 </b-container>

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded :src="require('../assets/Designs/ImgFive.jpg')" width="450px" height="500px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded :src="require('../assets/Designs/ImgSix.jpg')" width="430px" height="500px"></b-img>
    </b-col>
  </b-row>
 </b-container>

 

 <template v-slot:modal-footer>
        <b-button variant='warning' size='md' class='float-right' @click='showDg=false'>Close</b-button>
 </template>
        
 <template #modal-header>
     <div class="w-100">
          <span class="text-center" style="color:#00c2cb;font-family:'Montserrat-Regular'"> <h1> Lettering Designs </h1> </span>
          <span class="text-center" style="font-family:'Montserrat-Regular'"><h6> <i>Expressing myself through art!</i> </h6> </span>
     </div>
 </template>
 </b-modal> 
      
  
  </div>
</template>

<script>

export default {
    data() {
    return {
      showDg: false,
    };
  },
}
</script>

<style>
  


</style>
