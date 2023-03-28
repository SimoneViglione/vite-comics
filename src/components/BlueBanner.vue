<script>
export default {

data () {
  return {
    market: [
        {
            icon: 'buy-comics-digital-comics',
            product: 'DIGITAL COMICS'
        },
        {
            icon: 'buy-comics-merchandise',
            product: 'DC MERCHANDISE'
        },
        {
            icon: 'buy-comics-subscriptions',
            product: 'SUBSCRIPTION'
        },
        {
            icon: 'buy-comics-digit-shop-locator',
            product: 'COMIC SHOP LOCATOR'
        },
        {
            icon: 'buy-comics-power-visa',
            product: 'DC POWER VISA'
        },
    ]
    }},
    methods: {
        getImagePath: function (icon) {
            return new URL(`../assets/img/${icon}`, import.meta.url).href;
        }
    }
}
       
</script>

<template>
    <div class="blue-banner d-flex">
        <div v-for="item in market" :key="item.product" class="market d-flex">
            <div class="product-img">
               <img :src="getImagePath(item.icon)"> 
            </div>
            
            <h3>{{ item.product }}</h3>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.blue-banner {
    height: 200px;
    background-color: rgb(2, 130, 249);
    justify-content: center;
}

.market {
    align-items: center;
    gap: 1rem;
}

.product-img {
    width: 70px;
    height: 100px;

        img {
            width: 100%;
            height: 100px;
            margin: 0 10px;
        }
}
</style>