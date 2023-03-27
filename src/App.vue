<script>


import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';


export default {

  components: {TheHeader, TheFooter} 

}

</script>

<template>

  <TheHeader />
  
  <main>
    <h1>COMING SOON...</h1>
  </main>

  <TheFooter />
</template>

<style lang="scss">
  @use "./styles/general.scss";

  .d-flex {
    display: flex;
  }

  main {
    background-color: black;
    color: white;
    height: 100px;
  }

</style>
