<template>
  <div id="access">
     <b-card v-b-modal.modal-xl variant="primary"
     @click='show=true'
    title="Access Management System"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 30rem; height: 24rem; backgroundColor: #F7E06C; color:white; font-family: 'Montserrat-Regular'"
    class="mb-2 shadow border-0"
    footer-tag="footer"
    footer-bg-variant="light"
 
  >
   <b-img :src="require('../assets/AMS/AM.png')" class="mt-3" width="320px" height="200px"> </b-img>
   
    <b-modal id="modal-xl" size="xl" v-model='show' >
        <h2 class="desc mt-3"><u class="under">Overview</u></h2>
        <p class="desc ml-5 mr-5" style="font-size:19px"> Access Management System is an application that manages the lifecycle of access tokens. 
          An Access token is a means of access through which a customer can access the bank. It could be a Debit Card, Mobile Device or a PIN5. This application falls at heart of Identity and Access Management domain of the bank. This application has the highest CIA rating.</p>

        <b-img center :src="require('../assets/AMS/concept.png')" class="img-fluid" width="800px" height="400px"> </b-img>
   
    <b-table-simple borderless small >
      <b-tbody >
       <b-tr style="font-family:'Montserrat-Regular'">
        <b-th class="text-right"> <h5> <u> My Roles </u></h5> </b-th>
        <b-th class="text-left"> <h5> <u> Frameworks </u></h5></b-th>
       </b-tr>
       <b-tr>
         <b-td class="text-right">Frontend Developer</b-td>
         <b-td  class="text-left">VueJS</b-td>
       </b-tr>
         <b-tr>
         <b-td class="text-right">UI Designer</b-td>
         <b-td  class="text-left">Figma</b-td>
       </b-tr>
      <b-tr>
         <b-td class="text-right">DevOps Engineer</b-td>
         <b-td  class="text-left">Azure DevOps</b-td>
       </b-tr>
      </b-tbody>
    </b-table-simple>
<br><br>

     <h2 class="desc"><u class="under">Research</u></h2>
        <p class="desc ml-5 mr-5" style="font-size:19px">
          I took a survey and held semi-structured interviews with the users of the application to understand their expectations from the application. The survey was created in a way
          to understand how frequently the application will be used and what all features must be covered in the solution along with their priorities.
        </p>

       <p class="desc ml-5 mr-5" style="font-size:19px">
          As the users of the application were the bank shop employees, I mapped what actions can they take on behalf of the customers
          of the bank and what details will they be able to view. <br>I mapped actions and views under each category of an access token.
        </p>
                
        <b-img center :src="require('../assets/AMS/map.jpg')" class="img-fluid" width="900px" height="500px"> </b-img>
    <br><br>
        <p class="desc ml-5 mr-5" style="font-size:19px">
        Below is a pie chart addressing how frequently is the application being used:    
      </p>
    <b-img center :src="require('../assets/AMS/chart.png')" class="img-fluid" width="380px" height="300px"> </b-img>

  <br><br><br>
       <p class="desc ml-5 mr-5" style="font-size:19px">
       In order to explain one of the features, here is a use-case scenario:   
      
 <b-img center :src="require('../assets/AMS/useCase.png')" class="img-fluid" width="800px" height="440px"> </b-img>
 </p> <br><br><br>
   <p class="desc ml-5 mr-5" style="font-size:19px">
          Based on my research, I was able to define our target state below:
        <b-img center :src="require('../assets/AMS/targetState.png')" class="img-fluid" width="450px" height="420px"> </b-img>
        <ul class="mt-1">
           <li>Seamless Experience: The ability to create a unified yet customizable user experience regardless of what the user is trying to achieve.</li>
           <li>Traceable and accountability: Any action performed that changes the status of the access token has be traceable and logged.</li>
           <li>Abstraction: The ability to easily plug in and out authentication solutions from various vendors for authentication without the need to do any integration work with each of the different applications and systems. </li>
           <li>Orchestration: The ability to digest context from various sources and take run-time decisions based on that context in order to influence the user journey in various applications. Context could be business related (e.g. allowed services), user-related (e.g. user preferences), security-related (e.g. trust level), or regulatory related (e.g. multi-factor authentication requirements). </li>
           <li>Standardization: The design, develpment and deployment processes should adhere to the standards of the bank.</li>
         </ul>
        </p>
   <br><br>
   <h2 class="desc"><u class="under">Design & Development</u></h2>
        <p class="desc ml-5 mr-5" style="font-size:19px">
          The design mockups were created using the design system of the bank on Figma. Screens were developed in VueJS framework along with Vue Bootstrap
          components.<br> Continuous Integration and Continuous Deployment were achieved using Azure DevOps pipelines.
          Due to automated delivery the time-to-market was reduced by 75%.<br>
          Code quality tools were integrated within the DevOps pipeline to deliver secure code that is adhering to the coding standards.<br>
          ServiceNow was used for core IT processes such as Incident, Problem, Change and Call management. The process was automated and integrated in the pipeline as well. 

        </p>
     <b-img center :src="require('../assets/AMS/screens.png')" class="img-fluid" width="900px" height="500px"> </b-img>
     <br><br>

   <h2 class="desc"><u class="under">Learnings</u></h2>
       

          <p class="desc ml-5 mr-5" style="font-size:19px">
         This project has been very dear to me as other than the amazing opportunities I recieved through this project,
         I also discovered my drive and passion towards User Experience design. I learnt :<br>
         <ul class="mt-1">
           <li>the importance and impact of an engaging user experience on business.</li>
           <li>component-based development approach.</li>
           <li>how to address complex taskflows in an agile way of working. </li>
           <li>confiding in my own abilities.</li>
        
         </ul>
         </p>
    
         <template v-slot:modal-footer>
        <b-button variant='warning' size='md' class='float-right' @click='show=false'>Close</b-button>
      </template>
        
         <template #modal-header>
        <div class="w-100">
          <span class="text-center" style="color:#00c2cb;font-family:'Montserrat-Regular'"> <h1> Access Management System </h1> </span>
        </div>
      </template>
      </b-modal> 
<template #footer >
      <span class="text-muted" style="font-family:'Montserrat-Regular'; font-size:14px;"> How to manage means of access a person has with the bank?  </span>
        <small class="text-muted">Development | Design | Automation</small>
      </template>
  </b-card>
  </div>
</template>

<script>

export default {
    data() {
    return {
      show: false,
    };
  },
}
</script>

<style>
.im{
  display: inline-flex;
  justify-content: center;
}  
.under{
  text-decoration-style: double;
  text-decoration-color: #F7E06C;
}
.edit{
   
  justify-content: center;
}
</style>
