<template>
  <div id="Photography">
      
      <figure v-b-modal.modalPh class="figure mr-5"  @click='showPh=true'>
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
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1uKInDFYG095rDRTAw08vRzkrTjZmOEy4" width="500px" height="350px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1vrVfdwAaczIawgy2tdGqX2GJGKHUDtve" width="500px" height="350px"></b-img>
    </b-col>
  </b-row>
 </b-container>

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1wKfAhytAC5_33TraUcrdNzugTe6CJN1k" width="500px" height="350px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1wN3TdO0zxRWdl1TYX8vj9xhNjlZwyjAI" width="500px" height="350px"></b-img>
    </b-col>
  </b-row>
 </b-container>
<b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1vBsFhBksMwYDSowVqSUqVptb0CsXtGvN" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
       <b-img rounded src="https://drive.google.com/uc?export=view&id=1vYBU176PaROre_1wKmgmP4cZjxr7u7b1" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
  </b-container>
  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1ulwmhKscxcaCpAwoQAZERRXe7ybaWBlt" width="400px" height="400px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1vW2PVya1Rn8kpvGAH52e-JTgazwq9C7f" width="400px" height="400px"></b-img>
    </b-col>
  </b-row>
 </b-container>

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1v06SkKGP9QgyDaA6TBL4kBJipBDOCuNv" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1uemxRnlh1udVd3vTq7Wwv2XCV2vspByR" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
 </b-container>

 <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1u9uMceqtGMbCcE_nQ-lp6YlpVaPZvdu4" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1vEsPYUCbHxI3aX8QoLvdT8Vs2m5iSH4W" width="400px" height="450px"></b-img>
    </b-col>
  </b-row>
 </b-container>
 
 <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1uwX7jZ0QPFF8beFlGipA7nxH6-I1CVHK" width="400px" height="450px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1usPdQH3JPeaeSWQkglPEIPd6pVencIun" width="400px" height="450px"></b-img>
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
