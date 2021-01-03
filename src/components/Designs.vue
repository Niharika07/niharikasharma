<template>
  <div id="Designs">
      
       <figure v-b-modal.modalDg class="figure ml-5"  @click='showDg=true'>
        <img
          src="https://drive.google.com/uc?export=view&id=1wF-8BpLiiivU7nck0wX_3s_MU9KVdXtf"
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
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1x27FtmHhzlks-EHakbzSlkaeJeOfBYKn" width="500px" height="350px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1xtxyhKYl63OQxVNxAerwekSMnMtJmdVY" width="500px" height="350px"></b-img>
    </b-col>
  </b-row>
 </b-container>
  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded class="mt-2" src="https://drive.google.com/uc?export=view&id=1xe8opMje_Ovd-1uRs_tio1e4JYI0rrnx" width="500px" height="480px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=1xkKd1vZDhewUtu2xrOoy8wk9TLpXhH_D" width="500px" height="500px"></b-img>
    </b-col>
  </b-row>
 </b-container>

  <b-container class="p-4 d-flex" style="justify-content:center">
  <b-row>
    <b-col>
     <b-img rounded src="https://drive.google.com/uc?export=view&id=1x3VmxFkJAMb3K7THY3eE2P8f0PGcINGJ" width="450px" height="500px"></b-img>
    </b-col>
    <b-col>
      <b-img rounded src="https://drive.google.com/uc?export=view&id=18DvGydwQxB23bnSPox-VYEi6a6GgPSH-" width="430px" height="500px"></b-img>
    </b-col>
  </b-row>
 </b-container>

 

 <template v-slot:modal-footer>
        <b-button variant='warning' size='md' class='float-right' @click='showDg=false'>Close</b-button>
 </template>
        
 <template #modal-header>
     <div class="w-100">
          <span class="text-center" style="color:#00c2cb;font-family:'Montserrat-Regular'"> <h1> Lettering Designs </h1> </span>
          <span class="text-center" style="font-family:'Montserrat-Regular'"><h6> <i>Expressing myself through my art!</i> </h6> </span>
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
