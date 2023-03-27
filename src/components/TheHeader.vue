<script>

export default {

data () {
  return {
    headerLinks: [
      {
        name: 'characters'
      },

      {
        name: 'comics'
      },

      {
        name: 'movies'
      },

      {
        name: 'TV'
      },

      {
        name: 'games'
      },

      {
        name: 'collectibles'
      },

      {
        name: 'videos'
      },

      {
        name: 'fans'
      },

      {
        name: 'news'
      },

      {
        name: 'shop'
      },
    ],
  };
},
}

</script>

<template>

  <header>

  
    <div class="header-container d-flex">
      <div class="logo-wrapper">
        <img src="../../public/img/dc-logo.png"/>
      </div>

      <ul class="header-link d-flex">
        <li v-for="link in headerLinks" :key="link.name">
          <a href="">{{ link.name }}</a>
        </li>
      </ul>

    </div>
  </header>
</template>

<style lang="scss" scoped>

.header-container {
  height: 100px;
  background-color: white;
  border: solid 1px blue;
  align-items: center;
  justify-content: space-evenly;
}

.logo-wrapper {
  height: 70%;
  

  img {
    height: 100%;
  }
}
  .header-link {
    list-style: none;
    gap: 10px;
    
  }
</style>