<script>
export default {

data () {
  return {
    market: [
        {
            icon: 'buy-comics-digital-comics.png',
            product: 'DIGITAL COMICS'
        },
        {
            icon: 'buy-comics-merchandise.png',
            product: 'DC MERCHANDISE'
        },
        {
            icon: 'buy-comics-subscriptions.png',
            product: 'SUBSCRIPTION'
        },
        {
            icon: 'buy-comics-shop-locator.png',
            product: 'COMIC SHOP LOCATOR'
        },
        {
            icon: 'buy-dc-power-visa.svg',
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
        <div v-for="(item, i) in market" :key="i" class="market d-flex">
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
}

.product-img {
    width: 50px;
    height: 50px;   
    margin: 0 1rem;

        img {
            margin-right: -10px;
            height: 100%;    

            &:last-child {
                width: 100%;
            }
    
        }
}
</style>