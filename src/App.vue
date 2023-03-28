<script>

import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import BlueBanner from './components/BlueBanner.vue';
import TheMain from './components/TheMain.vue';


export default {

  components: {TheHeader, TheFooter, BlueBanner, TheMain}, 

  data () {
    return {}
  },
  methods: {
    
  }
}

</script>

<template>

  <TheHeader />
  
  <main>
    <theMain />
    

    <BlueBanner />
  </main>

  <TheFooter />
</template>

<style lang="scss">
  @use "./styles/general.scss";
</style>
