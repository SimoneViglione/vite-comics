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
    ],
  };
},
}

</script>

<template>
  <footer>
    <div class="footer-nav d-flex">
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

      <div class="logo-bg">
        
      </div>

    </div>

    <div class="footer-banner d-flex">
      <button>SIGN-UP NOW!</button>
      <div class="social d-flex">
        <h3>FOLLOW US</h3>
        <ul class="d-flex">
          <li><i class="fa-brands fa-facebook"></i></li>
          <li><i class="fa-brands fa-twitter"></i></li>
          <li><i class="fa-brands fa-youtube"></i></li>
          <li><i class="fa-brands fa-pinterest"></i></li>
          <li><i class="fa-solid fa-location-dot"></i></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
  .footer-nav {
    height: 420px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat:no-repeat;

    li {
      font-size: 12px;
      margin: 5px 0;
    }

  }

  .footer-links {
    max-width: 400px;
    max-height: 300px;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 1rem;
    margin-left: 300px;
    margin-top: 100px;

      a {
        font-size: 12px;
        color: rgba(255, 255, 255, 0.807);
        cursor: pointer;

        &:hover {
          color: rgba(0, 98, 255, 0.64);
        }
     
      }

  }

  .logo-bg {
    margin-left: 650px;
    width: 350px;
    height: 350px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-size: cover;
    align-self: center;
    overflow: hidden;
  }

  .footer-banner {
    background-color: rgb(48, 48, 48);
    height: 100px;

    button {
      background-color: rgb(48, 48, 48);
      border: solid 2px blue;
      color: white;
      font-weight: 600;
      height: 40px;
      padding: 10px;
      align-self: center;
      margin-left: 300px;
      width: 140px;
      cursor: pointer;

        &:active {
          filter: grayscale(1);
        }

        &:hover {
          scale: 1.1;
        }

    }

    h3 {
      font-weight: 600;
      margin-right: 10px;
      color: rgb(2, 130, 249);
    }

    i {
      color: grey;
      margin: 0 8px;
      font-size: 25px;
      cursor: pointer;
    }
  }

  .social {
    align-items: center;
    margin-left: 40%;
  }

</style>