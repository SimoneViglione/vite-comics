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
    <h1>COMING SOON...</h1>

    <BlueBanner />
  </main>

  <TheFooter />
</template>

<style lang="scss">
  @use "./styles/general.scss";
</style>
