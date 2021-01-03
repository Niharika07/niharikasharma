<template>
  <div id="oss">
    <b-card v-b-modal.modalOSS variant="primary"
     @click='showOSS=true'
    title="Open Source in Organizations"
    img-alt="Image"
    img-top
    tag="article"
    style="width: 30rem; height:24rem; backgroundColor: #F56476; color:white; font-family: 'Montserrat-Light'"
    class="mb-2 shadow border-0"
     footer-tag="footer"
    footer-bg-variant="light"
    footer-class="abc"
  >
   <b-img :src="require('../assets/OSS/oss.png')" class="mt-3" width="230px" height="200px"> </b-img>

<b-modal id="modalOSS" size="xl" v-model='showOSS' >

<h2 class="desc mt-3"><u class="under">About the Project</u></h2>
<p class="desc ml-5 mr-5" style="font-size:19px">
The primary objective of this project was to learn about the <i>open source maturity</i> in organizations.<br>
Open source maturity is to understand how to assess the extent to which a company:
<oL>
  <li>Uses open source.</li> 
  <li>Contributes to existing projects.</li>
  <li>Releases software as open source.</li> 
  <li>Has internal management and governance for open source software.</li> 
</oL>
</p>
<p class="desc ml-5 mr-5" style="font-size:19px">
The team tried to explore and understand the factors that make open source projects successful at certain companies, and devise a self-assessment model for companies that aspire to become a mature open source organization. 
</p>

<h2 class="desc mt-3"><u class="under">Process Overview</u></h2>
<p class="desc ml-5 mr-5" style="font-size:19px">
  Open source is fast becoming an excellent channel for building rapport in the technical community as well as for attracting talented individuals to interesting projects, however, not all open source programs can be considered as successful. The team therefore wanted to analyze and understand what makes the program successful in certain organizations, and what lessons can be learned from them,  so that more organizations can start adopting practices and methodologies that can lead them to have a mature open source program. 
</p>

<b-img center :src="require('../assets/OSS/process1.png')" class="img-fluid" width="750px"> </b-img>
<h2 class="desc mt-3"><u class="under">Analysis</u></h2>
<p class="desc ml-5 mr-5 mt-2" style="font-size:19px">
 The team first analyzed existing Open Source Maturity Models for organizations, such as the Qualipso Open Maturity Model (OMM) to understand what could be a good framework for organizations to assess their program’s maturity level. 
 </p>

<p class="desc ml-5 mr-5" style="font-size:19px">
 The team also looked at existing open source programs across different organizations - some that are already part of the TODO group and some that are not. This helped the team to learn about the guidelines that the TODO group provides for organizations to run a successful open source program. 
</p>

<p class="desc ml-5 mr-5" style="font-size:19px">
Through our extensive research, we discovered that there were more than 20 evaluation methods for open source software but thier is still no easy method for organizations to self-assess their source maturity.
</p>


<h2 class="desc mt-3"><u class="under">Designing the survey</u></h2>
<p class="desc ml-5 mr-5" style="font-size:19px">
The team then designed a survey to gather insights on the use of Open Source in various organizations. 
</p>
<span class="d-flex" style="justify-content:center">35 Participants from 4 countries
<b-img  :src="require('../assets/OSS/participants.png')" class="img-fluid" width="450px"> </b-img>
</span>


<p class="desc ml-5 mr-5" style="font-size:19px">
We chose to perform a dipstick survey by asking developers, open source program managers, contributors, etc. on what they value most in their company’s open source programs.  The goal was to find out which attributes or qualities of the open source program they liked or disliked about their current organization, how easy it is for them to understand the open source policies at their organization, and what is their self-rated perception about the maturity of their organization.
</p>
<p class="desc ml-5 mr-5" style="font-size:19px">
A set of questions were thoughtfully chosen to determine the role of open source software in the respondent’s organization, and what kind of open source programs their organization supported. 
In the context of Open Source development, the respondents were asked to self-rate on 4 categories:<br>
<oL>
  <li>Inclusion and Transparency</li> 
  <li>Protocols and Processes</li>
  <li>Participation and Collaboration</li> 
  <li>Community and Feedback</li> 
</oL>
</p>

<h2 class="desc mt-3"><u class="under">Insights</u></h2>

<p class="desc ml-5 mr-5" style="font-size:19px">
Based on the responses, here is a percentage of participants for few listed activities from the 4 categories:
<b-img center :src="require('../assets/OSS/involvement.png')" class="img-fluid" width="650px"> </b-img>
</p>

<h2 class="desc mt-3"><u class="under">Conceptualize</u></h2>
<p class="desc ml-5 mr-5" style="font-size:19px">
 Finally, the team put together the concept of a quick assessment framework to enable organizations to self-assess their open source maturity level in a standardized way and we call this “SATMOOSM - A Self-Assessment Tool for Measuring Organizational Open Source Maturity.”  
</p>
<p class="desc ml-5 mr-5" style="font-size:19px">
The tool would consider maturity across multiple organizational areas that are key to building and retaining a successful open source culture, and generate a maturity score based on the weightage associated with each area. 
In the true spirit of open source, it would allow organizations and open source enthusiasts to even recommend new categories or remove outdated categories and vote on weightages and maturity levels from time to time. 
</p>
<p class="desc ml-5 mr-5" style="font-size:19px">
The first version that has been put together by the team considers weightages from different categories based on the relative importance and their associated perceptions towards an organization’s maturity as voted by individuals in the survey.<br>
You can view them here.
</p>

<p class="desc ml-5 mr-5" style="font-size:19px">
The tool would consider maturity across all these areas and give a maturity score.
<b-img center :src="require('../assets/OSS/assessment.png')" class="img-fluid mt-2" width="650px"> </b-img>
</p>
<p class="desc ml-5 mr-5" style="font-size:19px">
The team hopes that as more and more organizations perform an assessment, and as the system learns about different organizations, the open source community as a whole would benefit as it would find more mature organizations in the open source space. 
</p>
  <template v-slot:modal-footer>
        <b-button variant='warning' size='md' class='float-right' @click='showOSS=false'>Close</b-button>
      </template>
        
         <template #modal-header>
        <div class="w-100">
          <span class="text-center" style="color:#00c2cb;font-family:'Montserrat-Regular'"> <h1> Open Source in Organizations </h1> </span>
        </div>
      </template>
</b-modal>
<template #footer >
      <span class="text-muted" style="font-family:'Montserrat-Regular'; font-size:15px;"> How to measure Open Source maturity of organizations?  </span><br>
        <small > Research</small>
      </template>
  </b-card>
  </div>
</template>

<script>

export default {
     data() {
    return {
      showOSS: false,
    };
  },
}
</script>

<style>
  
.abc{

  color: black;
}

</style>
