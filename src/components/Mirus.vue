<template>
  <div id="mirus">
      <b-card
    title="MIRUS"
    img-alt="Image"
    img-top
    tag="article"
    style="width: 30rem; height:24rem; backgroundColor: #F8CED2; color:white; font-family: 'Montserrat-Regular'"
    class="workshop mb-2 shadow border-0"
     footer-tag="footer"
    footer-bg-variant="light"
    v-on:click="openDoc()"
  >
    <figure class="figure mt-3">
        <img
          src="../assets/MS.png"
          class="figure-img img-fluid z-depth-1"
          style="width: 200px; height: 200px"
        />
        
      </figure>
      
<template #footer >
      <span class="text-muted" style="font-family:'Montserrat-Regular'; font-size:15px;"> How to build a platform for community learning?  </span><br>
        <small class="text-muted"> Project Management</small>
      </template>
  </b-card>
  </div>
</template>

<script>

export default {
     methods: {
    openDoc() {
      window.location.href =
        "https://drive.google.com/file/d/1NvzhvgmafObKUZdQN5-n28CpjVBVh50t/view?usp=sharing";
    },
  },
}
</script>

<style>
  


</style>
