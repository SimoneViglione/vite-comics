<script>
export default {

data () {
  return {
    market: [
        {
            icon: '../../public/img/buy-comics-digital-comics',
            product: 'DIGITAL COMICS'
        },
        {
            icon: '../../public/img/buy-comics-merchandise',
            product: 'DC MERCHANDISE'
        },
        {
            icon: '../../public/img/buy-comics-subscriptions',
            product: 'SUBSCRIPTION'
        },
        {
            icon: '../../public/img/buy-comics-shop-locator',
            product: 'COMIC SHOP LOCATOR'
        },
        {
            icon: '../../public/img/buy-dc-power-visa',
            product: 'DC POWER VISA'
        },
    ],
    };
},}
       
</script>

<template>
    <div class="blue-banner d-flex">
        <div v-for="item in market" :key="item.product">
            <img :src="item.icon" alt="">
            <h3>{{ item.product }}</h3>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.blue-banner {
    height: 200px;
    background-color: rgb(2, 130, 249);
}
</style>