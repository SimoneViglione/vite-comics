<script>


import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';


export default {

  components: {TheHeader, TheFooter} 

}

</script>

<template>

  <TheHeader />
  
  <h1>ciao</h1>

  <TheFooter />
</template>

<style lang="scss">
  @use "./styles/general.scss"
</style>
