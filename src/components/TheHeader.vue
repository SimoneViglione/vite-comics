<script>

export default {

data () {
  return {
    headerLinks: [
      {
        name: 'CHARACTERS'
      },

      {
        name: 'COMICS'
      },

      {
        name: 'MOVIES'
      },

      {
        name: 'TV'
      },

      {
        name: 'GAMES'
      },

      {
        name: 'COLLECTIBLES'
      },

      {
        name: 'VIDEOS'
      },

      {
        name: 'FANS'
      },

      {
        name: 'NEWS'
      },

      {
        name: 'SHOP'
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
    gap: 10px;
    
      a {
        text-decoration: none;
        color: black;
        transition: color 1s ease;
      }

      a:hover {
        text-decoration: underline blue;
        color: blue;
      }

  }
</style>