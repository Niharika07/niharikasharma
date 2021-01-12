<template>
  <div id="mirus">
      <b-card
    title="MIRUS"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 30rem; height:24rem; backgroundColor: #F8CED2; color:white; font-family: 'Montserrat-Regular'"
    class="workshop mb-2 shadow border-0"
     footer-tag="footer"
    footer-bg-variant="light"
    v-on:click="openDoc()"
  >
   <b-img :src="require('../assets/MS.png')" class="mt-3" width="200px" height="200px"> </b-img>
      
<template #footer>
      <span class="text-muted" style="font-family:'Montserrat-Regular'; font-size:14px;"> How to build and manage a platform for community learning?  </span><br>
        <small class="text-muted"> Project Management</small>
      </template>
  </b-card>
  </div>
</template>

<script>

export default {
     methods: {
    openDoc() {
      window.open("https://drive.google.com/file/d/1NvzhvgmafObKUZdQN5-n28CpjVBVh50t/view?usp=sharing", "_blank");
    },
  },
}
</script>

<style>
  


</style>
