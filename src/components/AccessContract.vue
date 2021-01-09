<template>
  <div id="AccessContract">
      <b-card v-b-modal.modalAC variant="primary"
     @click='showAC=true'
    title="Access Contract"
     img-alt="Image"
    img-top
    tag="article"
    style="width: 30rem; height: 24rem; backgroundColor: #A8E5FF; color:white; font-family: 'Montserrat-Regular'"
    class="mb-2 shadow border-0"
     footer-tag="footer"
    footer-bg-variant="light"
  >
 <b-img :src="require('../assets/AC/AC.png')" class="mt-4" width="200px" height="190px"> </b-img>

    <b-modal id="modalAC" size="xl" v-model='showAC' >
 <h2 class="desc mt-3"><u class="under">About the Project</u></h2>
 <p class="desc ml-5 mr-5" style="font-size:19px">
   As part of this project, I redesigned a critical Internet Banking application that was developed 20 years back.<br> Access Contract contains data about agreements between a customer and the bank regarding digital banking, including the users who are authorised to act within digital banking on behalf of the customer, and about which actions they are authorised to perform. 
   <br>Access Contract is an application
   through which a customer of the bank can:<br>
 

<span class="ml-5" style="font-family:Voga-Medium; color:#F7E06C;font-size:50px">1.</span>
<span class="ml-2" style="font-size:22px">Enroll products to her digital banking account.</span>
<br>
  <b-img center :src="require('../assets/AC/products.png')" class="img-fluid" width="600px" height="500px"> </b-img>

<span class="ml-5" style="font-family:Voga-Medium; color:#F7E06C;font-size:50px">2.</span>
<span class="ml-2" style="font-size:22px">Set permissions or define tasks that can be performed on her linked products.</span>
<br>
  <b-img center :src="require('../assets/AC/permissions.png')" class="img-fluid" width="600px" height="500px"> </b-img>

<span class="ml-5" style="font-family:Voga-Medium; color:#F7E06C;font-size:50px">3.</span>
<span class="ml-2" style="font-size:22px">Put finance/monetary restrictions on products.</span><br>
<ul class="ml-5"><li class="ml-3"> Limit on a payment.</li><li class="ml-3">Co-sign a payment.</li></ul>

<span class="ml-5" style="font-family:Voga-Medium; color:#F7E06C;font-size:50px">4.</span>
<span class="ml-2" style="font-size:22px">List Userships.</span><br>
<ul class="ml-5"><li class="ml-3"> Authorize one or more users to her digital banking products.</li>
<li class="ml-3">List all actions those users can perform.</li></ul>
</p>
<br>
 <h2 class="desc mt-3"><u class="under">Design Process</u></h2>
 <br>
<b-img center :src="require('../assets/AC/designProcess.png')" class="img-fluid" width="800px" height="650px"> </b-img>
<br>
 <h2 class="desc mt-3"><u class="under">Considerations</u></h2>
<ul class="desc ml-5"  style="font-size:19px"><li class="ml-3"> Aligning with the new standards of the bank for authentication and authorization into the application.</li>
<li class="ml-3">Avoiding cognitive load for complex task flows.</li>
<li class="ml-3">Adhering to the design system of the bank to maintain consistency and be compliant.</li>
<li class="ml-3">Getting regular feedbacks for every design iteration.</li>
</ul>
<br>
 <h2 class="desc mt-3"><u class="under">Prototypes</u></h2>

 <span class="desc ml-5 mr-5" style="font-size:19px">Login Screens</span>
<b-img center :src="require('../assets/AC/loginScreens.png')" class="img-fluid" width="700px" height="650px" style="position:relative"> </b-img>
<br><br>
<span class="desc ml-5 mr-5" style="font-size:19px">Overview Screens</span>
<b-img center :src="require('../assets/AC/overviewScreens1.png')" class="img-fluid" width="700px" height="650px" style="position:relative"> </b-img>
<b-img center :src="require('../assets/AC/overviewScreens2.png')" class="img-fluid" width="700px" height="650px" style="position:relative"> </b-img>
<br><br>

<span class="desc ml-5" style="font-size:19px">FAQ Screen</span>
<b-img center :src="require('../assets/AC/faqScreen.png')" class="img-fluid" width="700px" height="650px" style="position:relative"> </b-img>
<br>

<h2 class="desc"><u class="under">Learnings</u></h2>
<p class="desc ml-5 mr-5" style="font-size:19px">
         This project became the stepping stone for me in the field of design. I learnt :<br>
         <ul class="mt-1">
           <li>the importance of reducing cognitive load which was very high in the legacy application.</li>
           <li>the significance of receiving constant feedbacks from the user.</li>
           <li>how to weigh priorities while making design decisions.</li>
           <li>effective communication.</li>
         </ul>
         </p>

      <template v-slot:modal-footer>
        <b-button variant='warning' size='md' class='float-right' @click='showAC=false'>Close</b-button>
      </template>
        
         <template #modal-header>
        <div class="w-100">
          <span class="text-center" style="color:#00c2cb;font-family:'Montserrat-Regular'"> <h1> Access Contract </h1> </span>
        </div>
      </template>
      </b-modal> 
      
<template #footer >
      <span class="text-muted" style="font-family:'Montserrat-Regular'; font-size:15px;"> Who can perform what actions on my digital products?  </span><br>
        <small class="text-muted"> Design | Automation</small>
      </template>
  </b-card>
  </div>
</template>

<script>

export default {
    data() {
    return {
      showAC: false,
    };
  },
}
</script>

<style>
  


</style>
