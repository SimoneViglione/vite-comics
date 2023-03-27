<script>

export default {

data () {
  return {
    footerLinks: [
      {
        name: 'DC COMICS',
        subLinks: [
        {
        subLink: 'characters'
        },
        {
        subLink: 'comics'
        },
        {
        subLink: 'movies'
        },
        {
        subLink: 'TV'
        },
        {
        subLink: 'Games'
        },
        {
        subLink: 'Videos'
        },
        {
        subLink: 'News'
        },
        ],
      },

      {
        name: 'DC',
        subLinks: [
        {
        subLink: 'Terms Of Use'
        },
        {
        subLink: 'Privacy policy(New)'
        },
        {
        subLink: 'Ad choices'
        },
        {
        subLink: 'Advertising'
        },
        {
        subLink: 'Jobs'
        },
        {
        subLink: 'Subscriptions'
        },
        {
        subLink: 'Talent Workshops'
        },
        {
        subLink: 'CPSC Certificates'
        },
        {
        subLink: 'Ratings'
        },
        {
        subLink: 'Shop Help'
        },
        {
        subLink: 'Contact Us'
        },
        ],
      },

      {
        name: 'SITES',
        subLinks: [
        {
        subLink: 'DC'
        },
        {
        subLink: 'MAD Magazine'
        },
        {
        subLink: 'DC Kids'
        },
        {
        subLink: 'DC Universe'
        },
        {
        subLink: 'DC Power Visa'
        },
        ],
      },

      {
        name: 'SHOP',
        subLinks: [
        {
        subLink: 'Shop DC'
        },
        {
        subLink: 'Shop DC collectibles'
        },
        ],
      },      
    ],
  };
},
}

</script>

<template>
  <footer>
    <div class="footer-nav">
      <div class="footer-links d-flex">
        <div v-for="link in footerLinks" :key="link.name">
          <h4>{{ link.name }}</h4>
          <ul>
            <li v-for="(subLink, index) in link.subLinks" :key="index">
              <a>{{ subLink.subLink }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>

    <div class="footer-banner">

    </div>
  </footer>
</template>

<style lang="scss" scoped>
  .footer-nav {
    height: 300px;
    background-image: url(../../public/img/footer-bg.jpg);
    background-size: cover;
    background-repeat:no-repeat;
    color: white;
    
    ul {
      list-style: none;
    }

    li {
      font-size: 12px;
      margin: 5px 0;
    }

  }

  .footer-links {
    
    gap: 2rem;
    flex-wrap: wrap;

      a {
        font-size: 10px;
        color: rgba(255, 255, 255, 0.807);
      }

  }

</style>