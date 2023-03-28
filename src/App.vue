<script>


import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import BlueBanner from './components/BlueBanner.vue';


export default {

  components: {TheHeader, TheFooter, BlueBanner}, 

  data () {
    return {}
  },
}

</script>

<template>

  <TheHeader />
  
  <main>
    <div class="main-content">
      <h1>COMING SOON...</h1>
    </div>
    

    <BlueBanner />
  </main>

  <TheFooter />
</template>

<style lang="scss">
  @use "./styles/general.scss";

  .main-content {
    background-color: rgb(28, 28, 28);
    color: white;
    height: 100px;
  }
</style>
